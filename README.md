<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Matilda | Portfolio</title>
  <link rel="stylesheet" href="style (2).css">
</head>
<body>
  <header>
    <h1> Matilda's Portfolio</h1>
    <nav>
      <a href="#home">Home</a>
      <a href="#about">About Me</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <section id="home" class="container">
    <div>
      <img src="picture.jpg" alt="Profile Photo" class="profile-photo" onclick="showProfileModal()">
    </div>
    <div>
      <h2>Projects</h2>
      <div class="projects">
        <div class="card"><h3>Project One</h3><p>Female Empowerment Through Technology Workshop</p></div>
        <div class="card"><h3>Project Two</h3><p>Campus Digital Notice Board System</p></div>
      </div>
      <h2>Skills</h2>
      <div class="skills">
        <div class="card">HTML</div>
        <div class="card">CSS</div>
        <div class="card">javascript</div>
      </div>
    </div>
  </section>

  <section id="about" class="container">
    <div>
      <h2>About Me</h2>
      <p><i><i>My name is  Matilda cordor, and I am a proud student of Starz University, pursuing my undergraduate degree with a strong passion for growth, knowledge, and making a meaningful impact in the world around me.

I was born and raised in Liberia, in a home that valued education, discipline, and faith. Growing up, I was the kind of child who asked a lot of questions not just out of curiosity, but because I wanted to understand the world and how I could fit into it meaningfully. That spirit still drives me today.

My academic journey has been both challenging and rewarding. Starz University has become more than just a place of learning for me—it is a space where I am discovering who I am and what I am capable of. Through each lecture, project, and interaction, I am sharpening not only my academic skills but also my leadership, communication, and teamwork abilities.

Outside the classroom, I am passionate about self-development, technology, and uplifting others. I enjoy reading, helping classmates when I can, and participating in programs that promote positive change in the community. I believe that success is not just about personal achievement, but also about how much value we add to the lives of others.

Looking ahead, my goals are clear: to complete my education with excellence, to become a professional who leads with integrity, and to inspire other young girls to believe in themselves no matter where they come from or what challenges they face.

This is just the beginning of my story. I am still learning, still growing, and still building the woman I aspire to be.

</i>
    </p>
    </div>
  </section>

  <section id="contact" class="container">
    <div>
      <h2>Contact Me</h2>
      <form onsubmit="event.preventDefault(); showConfirmModal()">
        <input type="text" placeholder="Your Name" required>
        <input type="email" placeholder="Your Email" required>
        <textarea placeholder="Your Message" rows="4" required></textarea>
        <button type="submit">Send</button>
      </form>
    </div>
  </section>

  <footer>
    <p>&copy; 2025 Matilda | All rights reserved.</p>
  </footer>

  <!-- Profile Modal -->
  <div class="modal" id="profileModal">
    <div class="modal-content">
      <h2>About Me</h2>
     
      <button onclick="closeProfileModal()">Close</button>
    </div>
  </div>

  <!-- This is the Confirmation Modal -->
  <div class="confirm-modal" id="confirmModal">
    <div class="confirm-content">
      <p>Are you sure you want to submit this form?</p>
      <button onclick="submitForm()">Yes</button>
      <button onclick="closeConfirmModal()">No</button>
    </div>
  </div>
<!--This is my javascript-->
  <script>
    function showProfileModal() {
      document.getElementById('profileModal').style.display = 'flex';
    }
    function closeProfileModal() {
      document.getElementById('profileModal').style.display = 'none';
    }
    function showConfirmModal() {
      document.getElementById('confirmModal').style.display = 'flex';
    }
    function closeConfirmModal() {
      document.getElementById('confirmModal').style.display = 'none';
    }
    function submitForm() {
      closeConfirmModal();
      alert('Form submitted successfully!');
    }
  </script>
</body>
</html>

