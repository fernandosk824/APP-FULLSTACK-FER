<script>
export default {
  name: 'DashboardView',
}
</script>


<template>
  <header class="navbar">
      <div class="">
        <h1>Car Vendor</h1>
      </div>
      <nav>
        <ul>
          <li><a href="#">Home</a></li>
          <li><a href="#">Cars</a></li>
          <li><a href="#">About Us</a></li>
          <li><a href="#">Contact Us</a></li>
        </ul>
      </nav>
    </header>
    <main>
      <section id="banner" class="banner">
        <h2>Welcome to Car Vendor</h2>
        <p>
          We offer a wide selection of high-quality cars at competitive prices.
        </p>
        <a href="#" class="btn">View Our Cars</a>
      </section>
      <section id="featured-cars" class="featured-cars-section">
        <h2>Featured Cars</h2>
        <div class="featured-cars">

          <div class="car">
            <!-- <img src="car1.jpg" alt="Car 1" class="car-image" /> -->
            <div class="car-image car1"></div>
            <h3>2021 Toyota Camry</h3>
            <p>$25,000</p>
            <a href="#" class="btn">Learn More</a>
          </div>
          <div class="car">
            <!-- <img src="car2.jpg" alt="Car 2" class="car-image" /> -->
            <div class="car-image car2"></div>
            <h3>2021 Honda Accord</h3>
            <p>$26,000</p>
            <a href="#" class="btn">Learn More</a>
          </div>
          <div class="car">
            <!-- <img src="car3.jpg" alt="Car 3" class="car-image" /> -->
            <div class="car-image car3"></div>
            <h3>2021 Ford Mustang</h3>
            <p>$35,000</p>
            <a href="#" class="btn">Learn More</a>
          </div>
          <div class="car">
            <!-- <img src="car3.jpg" alt="Car 3" class="car-image" /> -->
            <div class="car-image car3"></div>
            <h3>2021 Ford Mustang</h3>
            <p>$35,000</p>
            <a href="#" class="btn">Learn More</a>
          </div>
        </div>
      </section>
      <section id="about" class="about">
        <h2>About Us</h2>
        <p>
          We are a family-owned car dealership that has been in business for
          over 20 years. We are committed to providing our customers with the
          best possible car buying experience.
        </p>
        <a href="#" class="btn">Learn More</a>
      </section>
      <section id="contact" class="contact">
        <div class="">
          <h2>Contact Us</h2>
        </div>
        <form action="submit-form.php" method="post">
          <label for="name">Name:</label>
          <input type="text" id="name" name="name" required />
          <label for="email">Email:</label>
          <input type="email" id="email" name="email" required />
          <label for="message">Message:</label>
          <textarea id="message" name="message" required></textarea>
          <button type="submit" class="btn">Send Message</button>
        </form>
      </section>
    </main>
    <footer>
      <p>Car Vendor &copy; 2023</p>
    </footer>
</template>


<style scoped>
/* Estilos Globales */
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

a {
  text-decoration: none;
  color: #000;
}

/* Estilos Barra de Navegación */

.navbar {
  background-color: #ffffff;
  font-size: 20px;
  font-weight: bold;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px;
}
.navbar div {
  display: flex;
  align-items: center;
  height: 100%;
}
.navbar div h1 {
  font-size: 30px;
  font-weight: bold;
  color: #000000;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
}


.navbar nav ul {
  display: flex;
  list-style: none;
}

.navbar nav ul li {
  margin-left: 20px;
}

.navbar nav ul li a {
  color: #000000;

  /* &:hover {
    color: #000;
  } */
}

.navbar nav ul li a:hover {
  color: #6b6b6b;
}

/* Estilos Banner */

.banner {
  height: 300px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background-image: url(../assets/background.jpg);
  background-size: cover;
  background-position: center center;
  background-repeat: no-repeat;
}

.banner h2 {
  font-size: 50px;
  font-weight: bold;
  color: #ffffff;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  text-align: center;
  display: inline;
}

.banner p {
  font-size: 20px;
  color: #ffffff;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  text-align: center;
}

.banner a {
  background-color: #757575;
  padding: 10px 20px;
  border-radius: 5px;
  color: #fff;
  font-size: 20px;
  font-weight: bold;
  margin-top: 20px;
}

.banner a:hover {
  background-color: #fff;
  color: #000000;
}

/* Featured Cars & Cars Section */

.featured-cars {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  padding: 50px;
}

.featured-cars-section h2 {
  font-size: 30px;
  font-weight: bold;
  color: #000000;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  margin-top: 20px;
  text-align: center;

}

.featured-cars .car {
  background-color: #ffffff;
  border-radius: 10px;
  box-shadow: 0 0 20px rgba(0, 0, 0, 0.4);
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin-bottom: 30px;

}

.car1 {
  background-image: url(../assets/toyota-camry.jpg);
}

.car2 {
  background-image: url(../assets/honda-accord.png);
}

.car3 {
  background-image: url(../assets/ford-mustang.jpg);
}

.featured-cars .car .car-image {
  /* overflow: hidden; */
  border-radius: 10px 10px 0 0;
  width: 400px;
  height: 170px;
  background-color: #6b6b6b;

  background-size: cover;
  background-position: center center;
  background-repeat: no-repeat;
}



.featured-cars .car h3 {
  font-size: 20px;
  font-weight: bold;
  color: #000000;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  margin: 15px 0;
}

.featured-cars .car p {
  font-size: 20px;
  color: #000000;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  margin-bottom: 10px;
}

.featured-cars .car a {
  background-color: #757575;
  padding: 10px 20px;
  border-radius: 5px;
  color: #fff;
  font-size: 20px;
  font-weight: bold;
  margin-bottom: 20px;
}

.featured-cars .car a:hover {
  background-color: #000;
  color: #fff;
}


/* About us section */

.about {
  display: flex;
  flex-direction: column;
  color: white;
  justify-content: space-between;
  align-items: center;
  padding: 50px;
  background-image: url(../assets/background.jpg);
  background-size: cover;
  background-position: center center;
  background-repeat: no-repeat;
}

.about h2 {
  font-size: 30px;
  font-weight: bold;
  color: #ffffff;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  margin-bottom: 20px;
}

.about p {
  font-size: 18px;
  color: #ffffff;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  text-align: justify;
  margin-bottom: 20px;
}

.about .btn {
  background-color: #757575;
  padding: 10px 20px;
  border-radius: 5px;
  color: #fff;
  font-size: 20px;
  font-weight: bold;
}

.about .btn:hover {
  background-color: #000;
  color: #fff;
}

/* Contact */
.contact {
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
  align-items: center;
  padding: 50px;
}

.contact div {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  /* border-right: 1px solid #000; */
  padding: 0 50px;
  margin-bottom: 20px;
}

.contact div h2 {
  font-size: 30px;
  font-weight: bold;
  color: #000000;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
}

.contact form {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
}

.contact form input,
.contact form textarea {
  padding: 10px;
  margin: 10px;
  border-radius: 5px;
  border: 1px solid #000;
  resize: none;
}

.contact form input:focus,
.contact form textarea:focus {
  outline: none;
  border: 1px solid #757575;
}

.contact form input {
  width: 300px;
}

.contact form textarea {
  width: 300px;
  height: 200px;
}

.contact form button {
  background-color: #757575;
  padding: 10px 20px;
  border-radius: 5px;
  color: #fff;
  font-size: 20px;
  font-weight: bold;
  margin-top: 20px;
}

.contact form button:hover {
  background-color: #000;
  cursor: pointer;
}

/* Footer */

footer {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 20px;
  background-color: #000;
  color: #fff;
}

footer p {
  font-size: 18px;
  font-weight: bold;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
}

@media screen and (min-width: 960px){
  .featured-cars {
    flex-direction: row; 
    flex-wrap: wrap;
  }

  .about p {
    width: 80%;
  }

  .contact {
    flex-direction: row;
  }
  
  .contact h2 {
    padding: 20px;
    border-right: 1px solid #000;
  }
}

@media screen and (min-width: 1200px){
  .about {
    flex-direction: row;
  }
  .about p {
    width: 900px;
    text-align: center;
  }
}

</style>

