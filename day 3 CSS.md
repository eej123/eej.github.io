/*   looks like is a second @media only screen and (max-width: 960px) statement provides logic for the script in html for
     conditions to get dynamic page reponse depending on toggle, click, or and the page size
     Unfortunately not well described in cut-paste day session.   */
@import url('https://fonts.googleapis.com/css?family=Open+Sans');
.avatar {
  border-radius: 50%; 
  float: right; 
  margin-right: 5em;
}
/* reset layout without padding and margins*/
body {
  padding: 0;
  margin: 0;
  /*background-image:url(BackgroundBadge.png)*/
} 

/* Begin with base font -top import statement part of this */
* {
  font-family: 'Open Sans', sans-serif;
}
header {
  height: 50px;
  background: #000;
  color: #fff;
  padding: 0 .5rem 0 1rem;
}
header .logo{
  line-height: 50px;
  font-weight: bold;
}
nav {
  float: right;
}
nav ul {
  margin: 0;
  padding: 0;
  list-style: none;
}
nav ul li {
  display: inline;
}
nav ul li a,
nav ul li a:link,
nav ul li a:visited {
  display: inline-block;
  padding: 0 .5rem;
  color: #fff;
  line-height: 50px;
  text-decoration: none;
}
nav ul li a:hover {
  background: #444;
}
main {
  /* Use a margin to center the page */
  margin: 0 auto;
  /* Set the width of the content */
  width: 960px;
  /* For smaller screens to not exceed the max screen width */
  max-width: 90%;
}
#toggleMenu {
    display: none;
  }
  @media only screen and (max-width: 960px)  {
    #toggleMenu {
      display: block;
      float: right;
      line-height: 50px;
    }
    nav {
      display: none; 
     }
    }
  @media only screen and (max-width: 960px)  {
    header {
      position: relative;
    }
  
    #toggleMenu {
      display: block;
      float: right;
      line-height: 50px;
    }
  
    header {
      position: relative;
    }
  
    nav {
      position: absolute;
      display: none;
      background: #000;
      top: 50px;
      left: 0;
      right: 0;
    }
  
    nav ul li a,
    nav ul li a:link,
    nav ul li a:visited{
      display: block;
      border-bottom: 1px solid #777;
    }
}
/*  sourceMappingURL=main.css.map */
