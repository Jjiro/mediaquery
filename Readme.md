MEDIA QUERY = FLEXBOX

- {
  margin: 5;
  padding: 5;
  }
  h1,
  body {
  margin: 5px;
  padding: 5px;
  background-color: beige;
  }
  h1 {
  text-align: center;
  color: red;
  }
  p {
  color: rgb(77, 77, 77);
  }

/**Container for flexboxes**/
section {
display: flex;
flex-wrap: nowrap;
}

/**Create two columns with 10px on both sides**/
.main {
flex: 40%;
padding: 10px;
}
.other {
flex: 40%;
padding: 10px;
}
.hidden {
text-align: center;
background-color: whitesmoke;
color: purple;
}

footer {
font-weight: bold;
text-align: center;
color: black;
}

/**Use 'all' or without for same result, 'screen', 'and' -- ','(or)**/
@media all and (max-width: 500px) {
h1 {
color: green;
}
footer {
color: green;
}
}

/**Use for 'print' only**/
@media print {
h1 {
color: pink;
}
p {
color: darkcyan;
}
footer {
color: pink;
}
}

/**For landscape and combining '@media (orientation: landscape) and (max-width: 500px)' {...}**/
@media (orientation: landscape) {
h1 {
color: brown;
}
p {
color: brown;
}
footer {
color: brown;
}
}

/**For portrait**/
/**@media (orientation: portrait) {
h1 {
color: blue;
}
p {
color: blueviolet;
}
footer {
color: blue;
}
}**/

/**Dealing with flexboxes**/
@media screen and (max-width: 500px) {
section {
flex-direction: column;
flex: 90%;
}
.main {
flex-direction: column;
}
.other {
flex-direction: column;
}
.hidden {
display: none;
}
}
