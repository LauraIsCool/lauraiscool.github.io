/* Code edited from: https://www.w3schools.com/html/tryit.asp?filename=tryhtml_layout_float */

<html lang="en">
<head>
<title>Laura Pemberton's Webpage</title>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
* {
  box-sizing: border-box;
}

body {
  font-family: Arial, Helvetica, sans-serif;
}

/* Style the header */
header {
  background-color: #c78fbc;
  padding: 30px;
  text-align: center;
  font-size: 35px;
  color: white;
}

/* Create two columns/boxes that floats next to each other */
nav {
  float: left;
  width: 30%;
  background: #948ca8;
  padding: 20px;
}

/* Style the list inside the menu */
nav ul {
  list-style-type: none;
  padding: 0;
  text-align: center;
}

article {
  float: left;
  padding: 20px;
  width: 70%;
  background-color: #eddae9;
}

/* Clear floats after the columns */
section:after {
  content: "";
  display: table;
  clear: both;
}

/* Style the footer */
footer {
  background-color: #c78fbc;
  padding: 10px;
  text-align: center;
  color: white;
}

@media (max-width: 600px) {
  nav, article {
    width: 100%;
    height: auto;
  }
}
</style>
</head>
<body>


<header>
  <h2>Laura Pemberton</h2>
</header>

<section>
  <nav>
    <ul>
      <li><a href="aboutme.html">About Me</a></li>
      <li><a href="#">New Page</a></li>
      <li><a href="#">New Page</a></li>
    </ul>
  </nav>
  
  <article>
    <p>Welcome to my GitHub website.</p>
  <p> Use the navigation bar to the left of this section to browse this website.</p>
  <a href="https://github.com/LauraIsCool"> Click here to access my GitHub page</a>
  </article>
</section>

<footer>
  <p>Footer</p>
</footer>

</body>
</html>




