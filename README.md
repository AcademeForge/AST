<html lang="en">
<!-- Moving Banner -->
<div style="width: 100%; background-color: #0a0a0a; color: white; padding: 5px 0; overflow: hidden; position: fixed; top: 0; left: 0; z-index: 10000;">
  <marquee behavior="scroll" direction="left" scrollamount="6" style="font-weight: bold; font-size: 14px;">
    IMPORTANT: Please click both buttons below — first, upload the Payment Screenshot, and then submit your Registration Details. Submitting both is mandatory for successful registration.
  </marquee>
</div>

<!-- Logo -->
<div class="logo-container">
    <a href="https://ibb.co/23qH49sJ" target="_blank">
        <img src="https://i.ibb.co/k2KvC79Z/IMG-20250320-164334-559.jpg" alt="AcademeForge Logo">
    </a>
</div>

<style>
    .logo-container {
        position: fixed;
        top: 70px;
        right: 15px;
        z-index: 10;
    }

    .logo-container img {
        height: 35px;
        width: auto;
        border-radius: 5px;
    }
</style>

<head>
  <meta charset="UTF-8">
  <title>AcademeForge Scholars Test Registration</title>
  <style>
    body { font-family: Arial, sans-serif; background: #00B4D8; padding: 20px; }
    form { max-width: 600px; margin: auto; background: #FF6B6B; padding: 20px; border-radius: 10px; }
    label { display: block; margin: 10px 0 5px; }
    input, select, textarea { width: 100%; padding: 8px; }
    button { margin-top: 20px; padding: 10px 20px; background: #00e5ff; color: white; border: none; border-radius: 5px; cursor: pointer; }
  </style>
</head>
<body>

<h2>AcademeForge Scholars Test Registration</h2>

<!-- Password Section -->
<div id="passwordSection" style="max-width: 600px; margin: auto; background: #ffffff; padding: 20px; border-radius: 10px;">
  <label for="accessPassword"><strong>Enter Password to Start Registration</strong></label>
  <input type="password" id="accessPassword" placeholder="Enter password to continue">
  <button onclick="checkPassword()">Submit Password</button>
  <p id="passwordMessage" style="color: red; margin-top: 10px;"></p>
</div>

<!-- Main Form Section -->
<div id="mainForm" style="display: none;">
  <form id="registrationForm" method="POST" enctype="multipart/form-data" action="https://script.google.com/macros/s/AKfycbxKUHRKkUA8Mt42QGrYR07fDye-tcs9R6_qkCJsv8osOpyG_gus6_9Xa7AyhzNjx84SpQ/exec">
    <label for="name">Full Name*</label>
    <input type="text" id="name" name="name" required>

    <label for="class">Class*</label>
    <select id="class" name="class" required>
      <option value="">Select Class</option>
      <option value="1">1</option><option value="2">2</option>
      <option value="3">3</option><option value="4">4</option>
      <option value="5">5</option><option value="6">6</option>
      <option value="7">7</option><option value="8">8</option>
      <option value="9">9</option><option value="10">10</option>
    </select>

    <label for="pincode">Pincode*</label>
    <input type="text" id="pincode" name="pincode" required>

    <label for="mode">Mode (Offline/Online)*</label>
    <select id="mode" name="mode" required>
      <option value="">Select Mode</option>
      <option value="Offline">Offline</option>
    </select>

    <label for="mobile">Mobile Number*</label>
    <input type="tel" id="mobile" name="mobile" required pattern="[0-9]{10}">

    <label for="email">Email Address*</label>
    <input type="email" id="email" name="email" required>

    <label for="gender">Gender*</label>
    <select id="gender" name="gender" required>
      <option value="">Select Gender</option>
      <option value="Male">Male</option><option value="Female">Female</option><option value="Other">Other</option>
    </select>

    <label for="dob">Date of Birth*</label>
    <input type="date" id="dob" name="dob" required>

    <label for="school_name">School Name*</label>
    <input type="text" id="school_name" name="school_name" required>

    <label for="school_address">School Address*</label>
    <textarea id="school_address" name="school_address" rows="3" required></textarea>

    <p style="margin-top: 15px;"> 
      <strong style="color: #d5ff05;">Registration fee submission:</strong></p>

    <!-- UPI Pay Button -->
    <a href="upi://pay?pa=6205176080@fam&pn=Devraj+Kumar&mc=0000&tid=1234567890&tr=1234567890&tn=Test+Payment&am=100&cu=INR" 
       target="_blank">
       <button type="button">Pay ₹99 Now</button>
    </a>
    <p style="margin-top: 10px; color: #555;">(Works only on mobile with UPI apps like GPay, PhonePe, Paytm, etc.)</p>
    <p style="margin-top: 15px;">If Blocked from the link pay manually using UPI ID: <strong style="color: #222;">devrajkumar01@ybl</strong></p>

    <strong style="color: #0c18f6;">Verify your name,number & upload payment screenshot:</strong>

    <iframe 
      data-tally-src="https://tally.so/embed/w5rWWE?alignLeft=1&hideTitle=1&transparentBackground=1&dynamicHeight=1" 
      loading="lazy" 
      width="100%" 
      height="90vh" 
      frameborder="0" 
      marginheight="0" 
      marginwidth="0" 
      title="Upload Screenshot">
    </iframe>

    <script>
      var d = document, s = d.createElement("script");
      s.src = "https://tally.so/widgets/embed.js";
      s.defer = true;
      d.body.appendChild(s);
    </script>

    <button type="submit">Submit</button>
  </form>
</div>

<script>
  function checkPassword() {
    const input = document.getElementById('accessPassword').value;
    const correctPassword = 'Password';
    if (input === correctPassword) {
      document.getElementById('passwordSection').style.display = 'none';
      document.getElementById('mainForm').style.display = 'block';
    } else {
      document.getElementById('passwordMessage').innerText = 'Incorrect password. Please try again.';
    }
  }
</script>

<style>
  footer {
    position: fixed;
    bottom: 0;
    left: 0;
    width: 100%;
    background: #5e60CE;
    color: white;
    text-align: center;
    padding: 1px 1cap;
    font-size: 65%;
    box-shadow: 0 -2px 10px rgba(5, 24, 101, 0.3);
    z-index: 777;
  }

  footer .social-links a {
    color: white;
    text-decoration: none;
    margin: 0 8px;
    font-weight: bold;
  }

  footer .social-links a:hover {
    color: #F1FAFF;
    text-decoration: underline;
  }
</style>

<footer>
  <div class="social-links">
    <a href="https://www.youtube.com/@AcademeForgePro" target="_blank">YouTube</a> |
    <a href="https://www.instagram.com/academeforgee" target="_blank">Instagram</a> |
    <a href="https://t.me/addlist/CVX57k_dpG4wNGJl" target="_blank">Join Telegram</a>
  </div>
  <p>&copy; 2025 AcademeForge. All rights reserved.</p>
</footer>