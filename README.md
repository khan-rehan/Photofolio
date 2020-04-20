# Photofolio [![Netlify Status](https://api.netlify.com/api/v1/badges/1530e16b-f6f9-4a73-ac56-f8fcb9c5b031/deploy-status)](https://app.netlify.com/sites/thephotofolio/deploys)

## A minimal portfolio template for Photographers!

To view a demo example, [click here](https://thephotofolio.netlify.app)

# Getting Started

## How to Use 🔧

From your command line, first clone Photofolio:

```
# Clone this repository
$ git clone https://github.com/khan-rehan/Photofolio.git

# Go into the repository
$ cd devio

# Remove current origin repository
$ git remote remove origin
```

# Template Instructions:

# Step 1 - STRUCTURE

Go to `index.html` and fill your information, they are 5 sections:

# Header section

- In `<table>` tag, go to first `<td>` tag with id `#logo` and put your name there.

```
<header id="header" class="animated slideInDown" style="animation-delay:1.8s;">
    <!---Nav bar--->
        <table>
            <tr>
                <td id="logo">[Your name]</td>
                <td id="navigation">
                    <a href="">Home</a>
                    <a href="#bio">About</a>
                    <a href="#work">Multimedia</a>
                    <a href="#contact">Contact</a>
                </td>
            </tr>
        </table>
    <!--End of navbar-->
</header>
```

# Home section

- In `<td>` tag id `#about`, go to `<h1>` and put your current project name there.
- Now, in `<p>` tag of the same, Describe about your current project.
- Below `<p>` tag, there's a `<button>` tag with an attribute `onclick` Put your resume link or any link of your publication you wanna display to visitors
  `eg - "location.href='your-link'"` and change the respective name of button in that tag.

```
<!-- Home section-->
    <table id="top_part">
        <tr>
            <td id="about" class="animated slideInLeft" style="animation-delay:2s;">
                <h1>[Your] Current Project/Research/Assignment</h1>
                <p>Describe your Project/Research/Assignment</p>
                <button onclick="location.href='!#'" type="button" class="btn_one">
                    Resume/Publication</button>
                <table>
                    <tr>
                        <td class="animated zoomIn" style="animation-delay:2.2s;"><a class="social" href="https://www.facebook.com/"><i class="fab fa-facebook"></i></a></td>
                        <td class="animated zoomIn" style="animation-delay:2.4s;"><a class="social" href="https://twitter.com/explore"><i class="fab fa-twitter"></i></a></td>
                        <td class="animated zoomIn" style="animation-delay:2.6s;"><a class="social" href="https://www.instagram.com/"><i class="fab fa-instagram"></i></a></td>
                    </tr>
                </table>
            </td>
            <td id="rightImage" class="animated jackInTheBox" style="animation-delay:2.2s;">
            </td>
        </tr>
    </table>
<!-- End of Home section-->
```

- To change the home section right-side image,go to `index.css` paste the image source in `url("imagesource")` of `#rightImage` on **166th** line of `index.css` source code

## Note:- image source can be written as `"img/yourimage"` & remember picture should be present in `img/` folder or you can paste a link of image/picture in that directly.

```
#rightImage {
    width:100%;
    height:95vh;
    background:linear-gradient(0deg,rgba(255, 44, 90, 0.8),rgba(2255, 44, 90, 0.8)),url("img/profile.jpg") center center;
    background-size:cover;
    background-repeat:no-repeat;
}
```

# About section

- on `<p>` tag in `<div>` with id `#bio`, describe about yourself

```
<!---about-->

    <div id="bio">
        <h1>About</h1>
        <p>
          Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.
        </p>
    </div>

<!---end of about-->
```

# Work section

- In `<img>` tag of `<div>` with id `#photos`, fill the `src`
  property with your portfolio pictures, your picture must be located inside `img/` folder.

## Note:- You can add as many pictures you want just copy & paste that `<img>` in `<div id = "photos">` tag for a new portfolio image and do the above mentioned steps☝🏻☝🏻☝🏻

```
<!-- Work--->
    <div id="work">
        <h1>Multimedia</h1>

  <!--Photos-->
        <div id="photos">
            <img onclick="magnify($(this).attr('src'))" src="img/1.jpg">
            <img onclick="magnify($(this).attr('src'))" src="img/2.jpg">
            <img onclick="magnify($(this).attr('src'))" src="img/3.jpg">
          </div>
    </div>
  <!--End of Photos-->
<!--End of Work-->
```

# Contact section

- In `<table>` tag with id `#inner_table`, there's a `<td>` tag for phone no. , email, fax no. , address so fill that with yours respective one's, also write your respectives after `&nbsp`
- In the same `<table>` tag, there's `<a>` tag with class `.social` having an attribute `href` fill that with your respective social links for every `<a>` tag.

## Note:- As of now the contact from is now working but i'll definitely upload the working contact form source code soon, Thankyou.

```
<!---Contact-->

    <div id="contact">
        <h1>contact</h1>
            <table>
                <tr>
                    <td>
                        <div id="inner_div">
                            <table id="inner_table">
                                <tr>
                                    <td><i class="fas fa-phone"></i>
                                    &nbsp; +1-202-555-0196
                                    </td>
                                </tr>
                                <tr>
                                    <td><i class="fas fa-at"></i>
                                    &nbsp; xyz@gmail.com
                                    </td>
                                </tr>
                                 <tr>
                                    <td><i class="fas fa-fax"></i>
                                     &nbsp; +1-202-555-0167
                                     </td>
                                </tr>
                                <tr>
                                    <td><i class="fas fa-map-marker-alt"></i>
                                    <div id="address">
                                        4726  Maxwell Farm Road<br>
                                        City,<br>
                                        Country.
                                    </div>
                                    </td>
                                </tr>
                                <tr>
                                    <td>
                                        <a class="social" href="https://www.facebook.com/"><i class="fab fa-facebook"></i></a>

                                        <a class="social" href="https://twitter.com/explore"><i class="fab fa-twitter"></i></a>

                                        <a class="social" href="https://www.instagram.com/"><i class="fab fa-instagram"></i></a>

                                    </td>
                                </tr>
                            </table>
                        </div>
                    </td>
                    <td>
                        <form>
                            <input type="text" placeholder="name" required>
                            <input type="email" placeholder="email" required><br>
                            <textarea placeholder="your message" required rows="5"></textarea><br>
                            <button class="btn_one">send</button>
                        </form>
                    </td>
                </tr>
            </table>
    </div>

<!---End of Contact-->
```

# Deployment 📦

Once you have done with your setup. You need to put your website online!

I highly recommend to use [Netlify](https://www.netlify.com) to achieve this on the EASIEST WAY

Please watch step-by-step the video tutorial to successfully upload your DevIO Website on Netlify!

[WATCH NOW STEP-BY-STEP TUTORIAL FOR DEPLOYMENT](https://youtu.be/tTKnuVx5qWA)
