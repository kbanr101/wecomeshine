---
layout: default
title: We Come Shine
---

<style>
  .home-hero {
    background: url('https://images.unsplash.com/photo-1610913365113-287c37f75b9e?auto=format&fit=crop&w=1400&q=80') center center / cover no-repeat;
    color: black;
    padding: 5rem 2rem;
    text-align: center;
    text-shadow: 1px 1px 3px rgba(0,0,0,0.7);
  }

  .home-hero h1 {
    font-size: 2.5rem;
    margin-bottom: 1rem;
  }

  .home-hero p {
    font-size: 1.25rem;
    margin-bottom: 2rem;
  }

  .cta-btn {
    display: inline-block;
    background-color: #ffc107;
    color: #000;
    padding: 1rem 2rem;
    font-weight: bold;
    font-size: 1.1rem;
    border-radius: 6px;
    text-decoration: none;
    transition: background 0.3s;
  }

  .cta-btn:hover {
    background-color: #ffb300;
  }

  .section {
    max-width: 800px;
    margin: 2rem auto;
    padding: 1rem;
    text-align: center;
  }

  .section h2 {
    font-size: 1.8rem;
    margin-bottom: 1rem;
  }

  .section ul {
    text-align: left;
    display: inline-block;
    margin: auto;
  }

  .badge-box {
    background: #e6f2ff;
    padding: 1rem;
    border-left: 4px solid #1e90ff;
    border-radius: 6px;
    margin-top: 1.5rem;
  }

  .testimonial-carousel {
    margin-top: 2rem;
    position: relative;
    height: 100px;
    overflow: hidden;
  }

  .testimonial-slide {
    opacity: 0;
    position: absolute;
    left: 0;
    right: 0;
    transition: opacity 0.8s ease-in-out;
  }

  .testimonial-slide.active {
    opacity: 1;
    position: relative;
  }

  .testimonial-slide p {
    font-style: italic;
    color: #444;
  }

  .testimonial-slide span {
    display: block;
    font-weight: bold;
    margin-top: 0.5rem;
    color: #555;
  }
</style>

<div class="home-hero">
  <h1>We Come Shine</h1>
  <p>Portland’s trusted mobile detailing service — and we’re giving away 1 month FREE to 5 winners.</p>
  <a href="./giveaway/" class="cta-btn" onclick="gtag('event', 'click', {'event_category':'Giveaway','event_label':'Homepage CTA'});">
  🎉 Enter the Giveaway
</a>


<div class="section">
  <h2>Why People Choose Us</h2>
  <ul>
    <li>✅ We come to your home, work, or wherever you are</li>
    <li>✅ Full interior & exterior service — not just a wash</li>
    <li>✅ Steam clean, leather care, fabric protection & more</li>
    <li>✅ Eco-friendly products & 100% satisfaction guarantee</li>
  </ul>

  <div class="badge-box">
    💡 <strong>New Customer Special:</strong> Everyone who enters the giveaway gets 60% OFF their first detail!
  </div>

  <div class="testimonial-carousel">
    <div class="testimonial-slide active">
      <p>“My car looked better than when I bought it. Super professional, came right to my driveway, and I didn’t lift a finger!”</p>
      <span>— Sarah, NE Portland</span>
    </div>
    <div class="testimonial-slide">
      <p>“Fast, spotless and friendly! I’ve used We Come Shine twice and won’t go back to the car wash.”</p>
      <span>— Marcus, Beaverton</span>
    </div>
    <div class="testimonial-slide">
      <p>“They even got the dog hair out of my trunk! Amazing attention to detail.”</p>
      <span>— Lily, Gresham</span>
    </div>
  </div>

  <a href="./giveaway/" class="cta-btn">🚗 Claim Your Free Month</a>
</div>

<script>
  let current = 0;
  const slides = document.querySelectorAll('.testimonial-slide');
  setInterval(() => {
    slides[current].classList.remove('active');
    current = (current + 1) % slides.length;
    slides[current].classList.add('active');
  }, 5000);
</script>
