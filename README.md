<<<<<<< HEAD
# introduction-to-play-framework

# play

### JPA

>  every JPA entity must provide an @Id property
> 
>  Don’t think about this provided id field as a functional identifier but as a technical identifier. It is generally a good idea to keep both concepts separated and to keep an automatically generated numeric ID as a technical identifier.
> 
> [JPA reference](http://play-framework.herokuapp.com/zh/jpa )

### mappedBy



    @OneToMany(mappedBy="post", cascade=CascadeType.ALL)
	public List<Comment> comments;
 
	public Post(User author, String title, String content) { 
	    this.comments = new ArrayList<Comment>();
	    this.author = author;
	    this.title = title;
	    this.content = content;
	    this.postedAt = new Date();
	}

> Note how we have used the mappedBy attribute to tell JPA that the Comment class’s post field maintains the relationship. When you define a bi-directional relation with JPA it is very important to tell it which side will maintain the relationship. In this case, since the Comments belong to the Post, it’s better that the Comment class maintains the relationship.

### yaml
[http://play-framework.herokuapp.com/zh/yaml](http://play-framework.herokuapp.com/zh/yaml "yaml")

### http

[http://play-framework.herokuapp.com/zh/routes#syntax](http://play-framework.herokuapp.com/zh/routes#syntax)

# jongo

[http://jongo.org/](http://jongo.org/)


# OpenAPI Specification

[http://swagger.io/specification/](http://swagger.io/specification/)
=======
# introduction-to-play-framework
>>>>>>> f5deb4b76fe0bcee8c243ba929e284d91b94ab61
