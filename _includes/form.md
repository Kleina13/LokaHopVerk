---
layout: default
title: form
---

<div class="register">
<fieldset>
<h1>WANNA JOIN ONE OF OUR CLUBS!?</h1>
<h2>Just fill in the form and you're good to go!!</h2>
<form>
    Which club?<br>
    <select name="club">
    <option value="riri">Rihanna Club</option>
    <option value="mb">Michael Bublé</option>
    <option value="mj">Michael Jackson</option>
    </select>
    First name:<br>
    <input type="text" name="firstname" required>
    <br>
    Last name:<br>
    <input type="text" name="lastname" required><br>
    E-mail:<br>
    <input type="text" name="mail" required><br>
    Phone number:<br>
    <input type="tel" name="phone number" title="Vinsamlegast skráið aðeins tölustafi" required><br>
    <br>
    Gender:<br>
    <input type="radio" name="gender" value="male" checked> Male<br>
    <input type="radio" name="gender" value="female"> Female<br>
    <input type="radio" name="gender" value="other"> Other<br>
    <br>
    When is your birthday?<br>
    <input type="date" data-date="" data-date-format="DD MMMM YYYY" required><br>
    <br>
    Subject: <br>
    <textarea id="subject" name="subject" placeholder="Write something.." style="height:200px"></textarea><br>
    <br>
    <input type="submit" value="Submit">
  </form>

<form>
    <legend></legend>
    <label>

    </label>
</form>
<form>
    <legend></legend>
    <label>
        
    </label>
</form>
<form>
    <legend></legend>
    <label>
        <input type="text">
    </label>
    <label>
        <input type="text">
    </label>
</form>
{% for artist in site.data.artist %}
    {{ artist.name }}
    {{ artist.spotify }}
    {{ artist.instagram }}
    <img src="../assets/images/{{ artist.image }}" alt="">
{% endfor %}