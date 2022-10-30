# HTML - Hyper Text Markup Language 

## INTRO 
> {not a programing language as it has no logical syntaxonly presentational aspects}

* Building block of any website
* Doesn't need a server 
* index.html is the root/hone page of the website for development

## Tag
```
<tagname> content </tagname>
<p> This is a paragraph </p>
<br/>   (self closing xhtml tag) - line break tag
<br>    (allowed in html5) - line break tag
<!DOCTYPE html> declaration not an html tag
```

## Inline V/s Block Level Elements
* Inline Elements : Don't start newline 
    `eg. <span> <img> <a>`
* Block Elements : Starts newline and takes whole space
    `eg. <div> <h1>-<h6> <p> <form>`
    
## HTML5 Semantics Tab : layout
- `header`
- `footer`
- `aside`
- `main`
- `article`
- `nav : nav-bar`
- `section`
- `details`

## Source Code Examples: 

<details>
  <summary>1. Use of basic tags</summary>
 
```
<!DOCTYPE html>
<html>
    <head>
        <title>
            Learning HTML
        </title>
    <head>

    <body>
        <!-- Headings -->
        <h1>Heading One</h1>
        <h2>Heading Two</h2>
        <h3>Heading Three</h3>
        <h4>Heading Four</h4>
        <h5>Heading Five</h5>
        <h6>Heading Six</h6>

        <a href="T02 - HTML5.html">Go to Blog</a>
        <br>
        <a href="#jump">Go to end</a>

        <!-- Paragraph -->
        <p>
            Lorem ipsum dolor <strong> sit amet </strong> consectetur adipisicing elit. Deserunt, odit.
        </p>
        <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. <em>officia voluptatem rem</em>  quibusdam ad distinctio sequi doloribus amet voluptate <a href="{url}" target="_blank"> Click here </a> nihil quos, enim perspiciatis, repudiandae animi. Doloribus ab sint voluptas neque.
        </p>

        <!-- LISTS -->
        <!-- Unordered List -->
        <ul>
            <li>List Item 1</li>
            <li>List Item 2</li>
            <li>List Item 3</li>
            <li>List Item 4</li>
        </ul>

        <!-- Ordered List -->
        <ol type="{1,i,I,A,a}">
            <li>List Item 1</li>
            <li>List Item 2</li>
            <li>List Item 3</li>
            <li>List Item 4</li>
        </ol>

        <!-- description list -->
        <dl>
            <dt>Apples</dt>
            <dd>- They are red.</dd>
            <dt>Oranges</dt>
            <dd>- They are orange.</dd>
        </dl>
        
        <!-- Tables -->
        <br>
        <table>
            <thead>
                <caption>Details Table</caption>
                <tr>
                    <th>Name</th>
                    <th>Email</th>
                    <th>Age</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>Ram</td>
                    <td>ram@abc.com</td>
                    <td>12</td>
                </tr>
                <tr>
                    <td>Ramesh</td>
                    <td>ramesh@abc.com</td>
                    <td>21</td>
                </tr>
                <tr>
                    <td>Sarah</td>
                    <td>Sarah@abc.com</td>
                    <td>18</td>
                </tr>
                <tr>
                    <td colspan="2">Sarah</td>
                    <td>18</td>
                </tr>
            </tbody>
        </table>
        
        <!-- break line --> <br>
        <!-- horizontal rule --> <hr>
        
        <!-- Forms (just look but no functionality)-->
        <form action="login" method="POST">
            <fieldset>
                <legend>Personal Details</legend>
            <div>
            <label for="firstName">First Name :</label>
            <input type="text" id="firstName" name="firstName" placeholder="Enter first name" size="30">
            </div>
            <br>
            <div>
            <label for="">Last Name</label>
            <input type="text" name="lastName" placeholder="Enter last name">
            </div>
            <br>
            <div>
            <label for="">Email</label>
            <input type="email" name="email">
            </div>
            <br>
            <div>
                <label for="">Message</label>
                <textarea name="message" rows="10" cols="30"> Enter the message</textarea>
            </div>
            <br>
            <div>
                <label for="">Gender</label>
                <select name="gender">
                    <option value="male">Male</option>
                    <option value="female">Female</option>
                    <option value="other">Other</option>
                </select>
            </div>
            <br>
            <div>
                <label for="">Age</label>
                <input type="number" name="age" value="30" min="0" max="50">
            </div>
            <br>
            <div>
                <label for="">DoB</label>
                <input type="date" name="dob">
            </div>
            <br>
            <div>
                <label for="">Password</label>
                <input type="password" name="password">
            </div>

            <!-- input types : file, checkbox, range, radio,  -->

            <br>
            <input type="submit" value="Submit">
            </fieldset>
        </form>

        <!-- Button -->
        <hr>
        <button click="">Click me</button>

        <!-- Images -->
        <br>
        <!-- a is anchor tag -->
        <!-- filepath= ../file.html goes to root directory and checks file.html there -->
        <a href="{url/filepath}">
            <img src="{url/filepath}" alt="Alt text" width="200px" height="200px" title="image">
        </a>

        <!-- Quotations -->
        <!-- Block Quote -->
        <blockquote cite="{url}">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Unde, consequuntur!</blockquote>

        <!-- Abbreviation -->
        <p>Lorem ipsum dolor <abbr title="World Wide Web">WWW</abbr> sit amet consectetur adipisicing elit. Aliquid, quo.</p>

        <!-- Citation -->
        <p><cite>HTML Cheat Sheet</cite> by V</p>

        <a name="jump">The End </a>
        <!-- Font styling -->
        <!-- b : bold -->
        <!-- i : itallics -->
        <!-- u : underlined -->
        <!-- small  -->
        <!-- big -->
        <!-- em -->
        <!-- strong -->
        <!-- sub : subscript -->
        <!-- sup : superscript -->

        <!-- Escape Characters -->
        <!-- &nbsp : " " --> &nbsp;
        <!-- &#8482 : TM--> &#8482;
        <!-- &amp : &--> &amp;
        <!-- &copy; Copright--> &copy;
        <!-- &lt : < --> &lt; 
        <!-- &gt : > --> &gt;
        <!-- &#63 --> &#63;
      
        <div style="margin-top:50px;"></div>
    </body>
</html>
```
</details>


<details>
  <summary>2. Making basic blog page with HTML5 Markup Tags</summary>
  
```
<!DOCTYPE html>
<html>
    <head>
        <title>Blog</title>
        <meta name="description" content="Awesome Blog Website by V">
        <meta name="keywords" content="web design blog, web dev blog, V">
        <style>
            #main-header{
                text-align: center;
                background-color: black;
                color: white;
                padding: 10px;
            }

            #main-footer{
                text-align: center;
                font-size: 18px;
            }
        </style>
    </head>

    <body>
        <header id="main-header">
            <h1>My Website</h1>
        </header>

        <a href="T01 - HTML Basics.html">Go to Cheat Sheet</a>
        
        <section>
            <article class="post">
                <h3>First Post</h3>
                <small>Posted on Jan 24</small>
                <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat corrupti accusantium beatae eum earum pariatur aspernatur mollitia laudantium nisi, et facere ad aliquid reprehenderit dolorum. Nam assumenda incidunt repellendus nostrum?
                </p>
                <a href="post.html">Read more</a>
            </article>

            <article class="post">
                <h3>Second Post</h3>
                <small>Posted on Jan 25</small>
                <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat corrupti accusantium beatae eum earum pariatur aspernatur mollitia laudantium nisi, et facere ad aliquid reprehenderit dolorum. Nam assumenda incidunt repellendus nostrum?
                </p>
                <a href="post.html">Read more</a>
            </article>

            <article class="post">
                <h3>Third Post</h3>
                <small>Posted on Jan 26</small>
                <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat corrupti accusantium beatae eum earum pariatur aspernatur mollitia laudantium nisi, et facere ad aliquid reprehenderit dolorum. Nam assumenda incidunt repellendus nostrum?
                </p>
                <a href="post.html">Read more</a>
            </article>
        </section>

        <aside>
            <h3>Categories</h3>
            <nav>
                <ul>
                    <li><a href="#">Category 1</a></li>
                    <li><a href="#">Category 2</a></li>
                    <li><a href="#">Category 3</a></li>
                </ul>
            </nav>
        </aside>

        <footer id="main-footer">
            <p>Copyright &copy; 2020, My Website</p>
        </footer>
    </body>
</html>
```
</details>

<details>
  <summary>3. Adding Media to simple webpage</summary>
  
```
<!DOCTYPE html>
<html>
    <head>
        <title> Media Page </title>
        <meta charset="UTF-8">
        <meta name="decsription" content="Awesome media page">
        <meta name="keywords" content="Media">
        <meta name="author" content="V">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <meta name="content-language" content="en-us">
    </head>

    <body style="background-color: salmon;">
        <header>
            <h1 style="color: green;">Media Page</h1>
            <hr>
        </header>
        <br>

        <main>
            <span>This is my block!</span>
            <div>
                <h3>First Article</h3>
                <small>Created on 27th Jan</small>
                <p style="color:blue; background-color: red;">
                    Lorem, ipsum dolor sit amet consectetur adipisicing elit. Ut repudiandae earum pariatur animi nobis quibusdam, odio eius mollitia incidunt iusto corrupti tempora est tenetur facilis? Nobis quia magni cupiditate quam.
                </p>
            </div>
            <div>
                <h3>Second Article</h3>
                <small>Created on 23th Jan</small>
                <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsa corporis praesentium quos delectus ullam, nihil est repellat a! Qui necessitatibus, veritatis excepturi quod quibusdam reiciendis quas veniam odio consequatur eos!
                </p>
            </div>    
            
            <!-- iframe -->
            <video src="{url/filepath}" poster="{thumbnail-url}" loop controls width="300px">Video was not found</video>
            
            <br>
            <iframe width="200px" src="{url}" frameborder="0" allowfullscreen></iframe>

            <br>
            <iframe width="200" heigh="200" src="T01 - HTML Basics.html" frameborder="1" name="disp1" id="disp1">Don't u see this?</iframe>

            <br>
            <a href="T02 - HTML5.html" target="disp1">Switch webpage</a>

            <!-- audio file .mp3 .wav .ogg -->
            <hr>
            <audio controls="audiocontrols" src=""></audio>

            <audio controls autoplay loop draggable="true">
                <source src="{url/filepath}.mp3">
                <source src="{url/filepath}.wav">
            </audio>
            <hr>

            <!-- video file -->
            <video width="200" height="200" controls>
                <source src="{url/filepath}.mp4">
                <source src="{url/filepath}.ogg">
            </video>


        </main>

        <footer>
            Copyright &copy; by V
        </footer>        
    </body>
</html>
```

</details>

<details>
  <summary>4. Adding colors to simple webpage</summary>
  
```
<!DOCTYPE html>
<html>
    <head>
        <title> Color Coding </title>
        <meta charset="UTF-8">
        <meta name="decsription" content="Awesome color coding page">
        <meta name="keywords" content="Color coding">
        <meta name="author" content="V">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <meta name="content-language" content="en-us">

        <!-- linking css -->
        <link rel="stylesheet" href="style.css">
    </head>

    <body>
        <header>
            <h1 style="color: green;">Color Coding</h1>
            <h2 style="color: rgb(60, 100, 100);">Color Coding</h2>
            <h3 style="color: #efefef">Color Coding</h3>
            <h4 style="color: rgba(120,220,1,11)">Color Coding</h4>
            <hr>
        </header>
        <br>

        <main>
            <span>This is my block!</span>
            <div>
                <h3>First Article</h3>
                <a href="T03 - Formatting.html" style="color: yellow; text-decoration: none;">Link to old page</a>
                <br/>
                <small>Created on 27th Jan</small>
                <p>
                    Lorem, ipsum dolor sit amet consectetur adipisicing elit. Ut repudiandae earum pariatur animi nobis quibusdam, odio eius mollitia incidunt iusto corrupti tempora est tenetur facilis? Nobis quia magni cupiditate quam.
                </p>
            </div>
            <div>
                <h3>Second Article</h3>
                <small>Created on 23th Jan</small>
                <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsa corporis praesentium quos delectus ullam, nihil est repellat a! Qui necessitatibus, veritatis excepturi quod quibusdam reiciendis quas veniam odio consequatur eos!
                </p>
            </div>    
            
        </main>

        <footer>
            Copyright &copy; by V
        </footer>        
    </body>
</html>
```

</details>
