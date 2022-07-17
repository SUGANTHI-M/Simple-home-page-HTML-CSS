This project is a simple home page consisting of a navigation bar and the content with search bar using HTML and CSS. 

HEADER SECTION:
HTML:
<nav>                           
     <img src="mainlogo.png" class="logo">
     <ul class="nav-links">
          <li><a href="">Home</a></li>
          <li><a href="">Courses</a></li>
          <li><a href="">Reviews</a></li>
          <li><a href="">Contacts</a></li>
          <li class="btn">Sign up</li>
      </ul>
</nav>  

<nav> tag - used for declaring the navigation section which contains navigation links, either within current document or to another document 
<img> tag - inserting the logo image 
<ul> tag     -  for navigational links as unordered list ( For ‘Sign up’, we are creating a button )


CSS:
#class ‘logo’ 
.logo
{
    margin-top: 15px;
    width:165px;
    height:100px;
}


#class ‘nav-links’
.nav-links{
    padding:28px 0;
}


.nav-links li{
    display: inline-block;
    margin: 0 15px;
}


#CSS property for first 4 elements (‘Home’, ’Courses’, ’Reviews’, ’Contacts’) of unordered list
#text 
.nav-links li a{
    text-decoration:none;
    color:black;
    padding:5px 0;
    position: relative;
}


#hover effect
.nav-links li a::after{
    content:'';
    background:#ff3d00;
    width:0;
    height:2px;
    position:absolute;
    bottom:0;
    left:0;
    transition: width 0.5s;
}


.nav-links li a:hover::after{
    width:100%;
}


#CSS property of ‘Sign Up’ button
.btn{
    background:#ff3d00;
    color: #fff;
    padding: 10px 30px;
    border-radius: 3px;
    cursor: pointer;
}


        
CONTENT SECTION:
The content section consists of a search bar and a list of courses below the search bar
            
HTML(search bar):            
<div class="content">
                <h1>Learn Courses Online</h1>
                <form>
                    <input type="text" placeholder="&#x270e; Enter keyword">
                    <button type="submit">Find Course</button>
                </form>


CSS(search bar):
#heading 
.content h1{
    font-size: 65px;
    font-weight: 600;
    margin-bottom: 40px;
}


#form layout(search bar)
.content form{
    background:#ff3d00;
    padding: 2px;
    border-radius: 2px;
    display:flex;
}


#input space of search bar
.content form input{
    flex:1;
    border:none;
    outline:none;
    padding: 0 20px;
    font-size: 18px;
}


#’Find Course’ button in search bar
.content form button{
    background:#ff3d00;
    color:#fff;
    padding:15px 40px;
    border: none;
    border-radius: 6px;
    cursor:pointer;
}
            
HTML(category list):
                <div class="category-list">
                    <div class="category">
                        <img src="logocategory.png">
                        <p>C</p>
                    </div>
                    <div class="category">
                        <img src="java1.png">
                        <p>Java</p>
                    </div>
                    <div class="category">
                        <img src="python.png">
                        <p>Python</p>
                    </div>
                    <div class="category">
                        <img src="html1.png">
                        <p>HTML</p>
                    </div>
                    <div class="category">
                        <img src="javascript1.png">
                        <p>Javascript</p>
                    </div>
                </div>


CSS(category list):
#class ‘category list’
.category-list{
    display:flex;
    align-items:center;
    justify-content: center;
    margin-top: 40px;
}




#class ‘category’
#Each courses in category list(text,background circle)
.category{
    width: 80px;
    height: 80px;
    border-radius: 50%;
    background: rgba(255,61,0,0.15);
    margin:0 10px;
    font-size: 12px;
    display: flex;
    align-items:center;
    justify-content: center;
    flex-direction: column;
}


#Image of each courses in category list
.category img{
    width:25px;
    margin-bottom: 5px;
}
