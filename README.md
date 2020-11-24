# Static Website: Tsunami Coffee

Use your knowledge of relative units and responsive web design to help Tsunami Coffee make their website come to life.

Throughout this project, you’ll edit the existing Tsunami Coffee website code so
that the website appears correctly on varying screen sizes. In addition, you’ll
contribute styles that will make this website more visually appealing.

![image](https://github.com/abemsq/tsunami-coffee-website/blob/master/image.png)

## HTML
```
<!DOCTYPE html>
<html>

<head>
  <title>The Tea Cozy</title>
  <link rel="stylesheet" href="style.css" type="text/css" />
</head>

<body>

  <!-- Header -->

  <header class="flex-container">
    <img src="https://content.codecademy.com/courses/freelance-1/unit-4/img-tea-cozy-logo.png" />
    <nav>
      <span><a href="#mission">Mission</a></span>
      <span><a href="#store">Featured Tea</a></span>
      <span><a href="#locations">Locations</a></span>
    </nav>
  </header>

  <!-- Main Content Container -->

  <div class="main">

    <!-- Mission Section -->

    <div id="mission" class="flex-container">
      <div class="content">
        <h2>Our Mission</h2>
        <h4>Handpicked, Artisanally Curated, Free Range, Sustainable, Small Batch, Fair Trade, Organic Tea</h4>
      </div>
    </div>

    <!-- Store Section -->

    <div id="store">
      <h2>Tea of the Month</h2>
      <h4>What's Steeping at The Tea Cozy?</h4>
      <div class="flex-container items">
        <div class="item">
          <img src="https://content.codecademy.com/courses/freelance-1/unit-4/img-berryblitz.jpg" />
          <span>Fall Berry Blitz Tea</span>
        </div>
        <div class="item">
          <img src="https://content.codecademy.com/courses/freelance-1/unit-4/img-spiced-rum.jpg" />
          <span>Spiced Rum Tea</span>
        </div>
        <div class="item">
          <img src="https://content.codecademy.com/courses/freelance-1/unit-4/img-donut.jpg" />
          <span>Seasonal Donuts</span>
        </div>
        <div class="item">
          <img src="https://content.codecademy.com/courses/freelance-1/unit-4/img-myrtle-ave.jpg" />
          <span>Myrtle Ave Tea</span>
        </div>
        <div class="item">
          <img src="https://content.codecademy.com/courses/freelance-1/unit-4/img-bedford-bizarre.jpg" />
          <span>Bedford Bizarre Tea</span>
        </div>
      </div>
    </div>

    <!-- Locations Section -->

    <div id="locations">
      <h2>Locations</h2>
      <div class="flex-container locations">
        <div class="location">
          <h3>Downtown</h3>
          <p>384 West 4th St</p>
          <p>Suite 108</p>
          <p>Portland, Maine</p>
        </div>
        <div class="location">
          <h3>East Bayside</h3>
          <p>3433 Phisherman's Avenue</p>
          <p>(Northwest Corner)</p>
          <p>Portland, Maine</p>
        </div>
        <div class="location">
          <h3>Oakdale</h3>
          <p>515 Crescent Avenue</p>
          <p>Second Floor</p>
          <p>Portland, Maine</p>
        </div>
      </div>
    </div>
  </div>

    <!-- Contact Section -->
    <div id="contact">
      <h2>The Tea Cozy</h2>
      <h5>contact@theteacozy.com</h5>
      <h5>917-555-8904</h5>
    </div>

    <!-- Footer Section -->
    <footer>
      <h5>copyright The Tea Cozy 2017</h5>
    </footer>
  </body>
</html>
```

## CSS
```
/* Universal Styles */

body {
  margin: 0;
  font-family: "Helvetica", sans-serif;
  color: seashell;
  background-color: black;
  font-size: 22px;
  text-align: center;
}

a {
  color: seashell;
}

h2,
h3,
h4 {
  margin: 0;
  padding: 10px;
}

.flex-container {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
}

/* Header Section */

header {
  width: 100%;
  position: fixed;
  z-index: 1;
  height: 69px;
  background-color: black;
  border-bottom: 1px solid seashell;
  align-items: center;
}

header img {
  height: 50px;
  padding-left: 10px;
}

nav {
  text-align: right;
  flex-grow: 1;
}

nav span {
  display: inline-block;
  padding: 20px 10px;
}

/* Main Section */

.main {
  padding-top: 69px;
  opacity: 0.9;
  width: 1200px;
  margin: auto;
}

/* Mission Section */

#mission {
  height: 700px;
  background-image: url("https://content.codecademy.com/courses/freelance-1/unit-4/img-mission-background.jpg");
  padding-top: 70px;
}

#mission .content {
  margin: auto;
  background-color: black;
  width: 100%;
}

/* Store Section */

#store {
  height: 700px;
  width: 1000px;
  margin: auto;
  padding-top: 70px;
}

.item {
  padding: 5px;
}

.item img {
  height: 200px;
  margin: 10px;
  display: block;
}

.item span {
  display: block;
  padding: 5px;
  font-weight: bold;
  text-align: center;
}

/* Location Section */

.flex-container.locations {
  padding-top: 5px;
}

#locations {
  background-image: url("https://content.codecademy.com/courses/freelance-1/unit-4/img-locations-background.jpg");
  height: 500px;
  padding-top: 70px;
}

#locations .flex-container {
  margin: auto;
  width: 1100px;
}

.location {
  opacity: 1.0;
  padding: 10px;
  margin: 5px 20px;
  background-color: black;
  flex-basis: 280px;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

/* Contact Section */

#contact {
  height: 200px;
}

/* Footer Section */

footer {
  text-align: left;
  padding-left: 20px;
}
```