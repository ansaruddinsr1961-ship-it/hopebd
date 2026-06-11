# hopebd
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>HopeBD - Helping Communities Together</title>

<style>
:root{
  --primary:#0f766e;
  --secondary:#22c55e;
  --dark:#0f172a;
  --light:#f8fafc;
}

*{
  margin:0;
  padding:0;
  box-sizing:border-box;
  font-family:Segoe UI, sans-serif;
}

body{
  background:var(--light);
  color:#333;
}

header{
  background:white;
  box-shadow:0 2px 10px rgba(0,0,0,.08);
  position:sticky;
  top:0;
  z-index:100;
}

.nav{
  max-width:1200px;
  margin:auto;
  display:flex;
  justify-content:space-between;
  align-items:center;
  padding:18px;
}

.logo{
  font-size:1.5rem;
  font-weight:bold;
  color:var(--primary);
}

.nav-links a{
  text-decoration:none;
  color:var(--dark);
  margin-left:20px;
  font-weight:500;
}

.hero{
  min-height:85vh;
  display:flex;
  align-items:center;
  justify-content:center;
  text-align:center;
  color:white;
  background:
  linear-gradient(rgba(0,0,0,.55),rgba(0,0,0,.55)),
  url('https://images.unsplash.com/photo-1488521787991-ed7bbaae773c?auto=format&fit=crop&w=1600&q=80');
  background-size:cover;
  background-position:center;
}

.hero-content{
  max-width:800px;
  padding:20px;
}

.hero h1{
  font-size:3.5rem;
  margin-bottom:20px;
}

.hero p{
  font-size:1.2rem;
  margin-bottom:30px;
}

.btn{
  display:inline-block;
  padding:14px 30px;
  background:var(--secondary);
  color:white;
  text-decoration:none;
  border-radius:8px;
  transition:.3s;
}

.btn:hover{
  transform:translateY(-3px);
}

.section{
  max-width:1200px;
  margin:auto;
  padding:80px 20px;
}

.section-title{
  text-align:center;
  margin-bottom:50px;
  color:var(--dark);
}

.stats{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(200px,1fr));
  gap:25px;
}

.stat{
  background:white;
  text-align:center;
  padding:30px;
  border-radius:15px;
  box-shadow:0 5px 15px rgba(0,0,0,.08);
}

.stat h2{
  color:var(--primary);
  margin-bottom:10px;
}

.cards{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
  gap:25px;
}

.card{
  background:white;
  padding:30px;
  border-radius:15px;
  box-shadow:0 5px 15px rgba(0,0,0,.08);
}

.card h3{
  margin-bottom:15px;
  color:var(--primary);
}

.cta{
  background:var(--primary);
  color:white;
  text-align:center;
  padding:80px 20px;
}

footer{
  background:var(--dark);
  color:white;
  text-align:center;
  padding:25px;
}

form{
  max-width:600px;
  margin:auto;
}

input, textarea{
  width:100%;
  padding:14px;
  margin-bottom:15px;
  border:1px solid #ddd;
  border-radius:8px;
}

button{
  background:var(--secondary);
  color:white;
  border:none;
  padding:14px 25px;
  border-radius:8px;
  cursor:pointer;
}

@media(max-width:768px){
  .hero h1{
    font-size:2.3rem;
  }

  .nav{
    flex-direction:column;
  }

  .nav-links{
    margin-top:15px;
  }
}
</style>
</head>

<body>

<header>
  <div class="nav">
    <div class="logo">HopeBD</div>

    <div class="nav-links">
      <a href="#about">About</a>
      <a href="#help">Programs</a>
      <a href="#donate">Donate</a>
      <a href="#contact">Contact</a>
    </div>
  </div>
</header>

<section class="hero">
  <div class="hero-content">
    <h1>Changing Lives Together</h1>
    <p>Connecting generous people with families who need support through transparent and community-driven assistance.</p>
    <a href="#donate" class="btn">Donate Now</a>
  </div>
</section>

<section class="section">
  <h2 class="section-title">Our Impact</h2>

  <div class="stats">
    <div class="stat">
      <h2>1,200+</h2>
      <p>Families Helped</p>
    </div>

    <div class="stat">
      <h2>500+</h2>
      <p>Volunteers</p>
    </div>

    <div class="stat">
      <h2>৳15L+</h2>
      <p>Donations Raised</p>
    </div>

    <div class="stat">
      <h2>25+</h2>
      <p>Communities Served</p>
    </div>
  </div>
</section>

<section class="section" id="help">
  <h2 class="section-title">How We Help</h2>

  <div class="cards">

    <div class="card">
      <h3>Food Assistance</h3>
      <p>Providing food packages and emergency support for struggling families.</p>
    </div>

    <div class="card">
      <h3>Education Support</h3>
      <p>Helping students with school fees, books and learning materials.</p>
    </div>

    <div class="card">
      <h3>Medical Aid</h3>
      <p>Supporting treatment costs and essential healthcare needs.</p>
    </div>

  </div>
</section>

<section class="cta" id="donate">
  <h2>Every Contribution Makes a Difference</h2>
  <br>
  <p>Join our mission to support vulnerable families.</p>
  <br>
  <a href="#contact" class="btn">Become a Volunteer</a>
</section>

<section class="section" id="contact">
  <h2 class="section-title">Contact Us</h2>

  <form id="contactForm">
    <input type="text" placeholder="Your Name" required>
    <input type="email" placeholder="Email Address" required>
    <textarea rows="5" placeholder="Your Message" required></textarea>
    <button type="submit">Send Message</button>
  </form>
</section>

<footer>
  <p>© 2026 HopeBD. All Rights Reserved.</p>
</footer>

<script>
document.getElementById('contactForm')
.addEventListener('submit', function(e){
    e.preventDefault();
    alert('Thank you! Your message has been received.');
});
</script>

</body>
</html>
