# Vansportfolio 
body{
  font-size: 16px;
  font-family: "Gill Sans", "Gill Sans MT", "Myriad Pro", "DejaVu Sans Condensed", Helvetica, Arial, "sans-serif";
background-color: #6C9E97;
}
section { 
  display: block;
}

html, body {
    width: 100%;
    height: 100%;
    margin: 0;
}
html {
    font-family: "helvetica neue", sans-serif;
}

.nav {
    border-bottom: 1px solid #EAEAEB;
    text-align: right;
    height: 20px;
    line-height: 20px;
}
.menu {
    margin: 0 10px 0 0;
}
.menu a {
    clear: right;
    text-decoration: none;
    color: gray;
    margin: 0 10px;
    line-height: 20px;
}



label {
    margin: 0 40px 0 0;
    font-size: 20px;
    line-height: 20px;
    display: none;
    width: 8px;
    float: right;
}
#toggle {
    display: none;
}
h1{
    color: silver;
	text-decoration: none;
	text-align: center;
	text-shadow: 2px 2px #ffffff;
	padding: 2 2 2 2;
}

h2{
	color:antiquewhite;
	text-decoration: underline;
	line-height: 1em;
	font-size: 15px;
	background: #000000;
	padding: 10px;
	text-align: center;
	margin:auto;
}


p{
	color: #282828;
	font-size: 12px;
	margin: auto;
	padding:auto;
	
}
img {
  border: 0 solid #ddd;
  padding: 10px;
  width: 150px;
align-content:center;
	
}

img:hover {
  box-shadow: 0 0 2px 1px rgba(0, 140, 186, 0.5);
}
/*--- Grid areas ---*/


main {
  grid-area: logo;
  
}

aside {
  grid-area: content;
}


section{
  grid-area: sponsors;
}

footer {
  grid-area: footer;
}
nav{
	grid-area: sidebar;
}


/*--- Grid parent ---*/
#content {
  display: grid;
  margin: 0 2rem;
	max-width: 960px;
  grid-gap: 2rem 1rem;
  grid-template-columns: 33.3%, 33.3%, 33.3%;
  grid-template-rows: 3rem auto;
  grid-template-areas:
          "logo menu menu"
          "content content sidebar"
          "sponsors sponsors sponsors"
          "footer footer footer";
}
main {
  list-style-type: none;
  padding: 0;
  font-size: 1.1rem;
  margin-right: 0.5rem;
}

main {
  margin-right: 0;
}

/*--- Sponsors ---*/
.sponsor {
  display: grid;
  grid-template-columns: repeat(5, 1fr):
 
  grid-template-rows: auto;
  grid-column-gap: 1rem;
}

.sponsor {
  margin-left: 0;
  margin-right: 0;
  background-color: #fff;
  border-radius: 0.625rem;
  display: inline-flex;
  align-items: center;
  justify-content: center;
}

@media only screen and (max-width: 500px) {
    label {
        display: block;
        cursor: pointer;
    }
    .menu {
        text-align: center;
        width: 100%;
        display: none;
    }
    .menu a {
        display: block;
        border-bottom: 1px solid #EAEAEB;
        margin: 0;
     
    }
    #toggle:checked + .menu {
        display: block;
    }
    
    
}

