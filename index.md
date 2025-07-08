---
layout: default
title: We Come Shine
---

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
    💡 <strong>New Customer Special:</strong> Everyone who enters the giveaway gets 10% OFF their first detail!
  </div>

  <div class="testimonial-carousel">
    <div class="testimonial-slide active">
      <p>“My car looked better than when I bought it. Super professional, came right to my driveway.”</p>
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
  <br>
  <br>

    <a href="./giveaway/" class="cta-btn" onclick="gtag('event', 'click', {'event_category':'Giveaway','event_label':'Homepage CTA'});">
  🎉 Claim Your free Month
</a>

<script>
  let current = 0;
  const slides = document.querySelectorAll('.testimonial-slide');
  setInterval(() => {
    slides[current].classList.remove('active');
    current = (current + 1) % slides.length;
    slides[current].classList.add('active');
  }, 5000);
</script>
