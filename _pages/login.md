---
layout: page
permalink: /login/
title: Log In / Sign Up
description: Log in to an existing account, or create a new account.
nav: true
nav_order: 3
---

<div class="card mt-3 wow fadeIn" data-wow-delay="1s" style="padding: 3rem;">
  <h2><b style="font-weight:800;">Log In</b></h2>
  <h6>Don't have an account yet? <a href="#Sign Up">Sign Up.</a></h6>
  <form action="{{ site.baseurl }}/spotify_search.html" method="get" id="search-ui">
    <!-- <label for="search-box">Search: </label> -->
    <i class="fas fa-user"></i> <input type="text" class="search-box" name="query" placeholder="π€ Username" target="">
    <br />
    <i class="fas fa-unlock"></i> <input type="password" class="search-box" name="query" placeholder="π Password"  target="">
    <button type="submit">
      <i class="fas fa-arrow-right"></i>
    </button>
    <!-- <input type="submit" value="π" id="search-button"> -->
  </form>
</div>

<br /><br />
<div class="card mt-3 wow fadeIn" data-wow-delay="1s" style="padding: 3rem;">
  <h2><a style="font-weight:800;margin-bottom:1rem;">Sign Up</a></h2>
  <h6><b style="font-weight:400;"><i class="fas fa-at"></i> E-MAIL / ι»ε­γ‘γΌγ«</b></h6>
  <form action="{{ site.baseurl }}/search.html" method="get" id="search-ui">
    <!-- <label for="search-box">Search: </label> -->
    <i class="fas fa-user"></i> <input type="text" class="search-box" name="query" placeholder="π€ Create Username" target="">
    <br />
    <i class="fas fa-unlock"></i> <input type="password" class="search-box" name="query" placeholder="π Create Password"  target="">
    <button type="submit">
      <i class="fas fa-arrow-right"></i>
    </button>
    <!-- <input type="submit" value="π" id="search-button"> -->
  </form>
  <br /><br /><br />
  <h6><b style="font-weight:400;"><i class="fas fa-phone"></i> PHONE NUMBER / ι»θ©±ηͺε·</b></h6>
  This is used for two-step verification, and alerts. Your phone number will not be stored, or sold to third parties.<br /><br />

  <form action="{{ site.baseurl }}/search.html" method="get" id="search-ui">
    <!-- <label for="search-box">Search: </label> -->
    <i class="fas fa-mobile"></i> <input type="text" class="search-box" name="query" placeholder="π Phone Number" target=""><br /><br /><br />
    <h6><b style="font-weight:400;"><i class="fas fa-phone"></i> ADDRESS / ι»θ©±ηͺε·</b></h6>
    <input type="text" class="search-box" name="query" placeholder="π  House Number" target=""><br />
    <input type="text" class="search-box" name="query" placeholder="π Address 1" target=""><br />
    <input type="text" class="search-box" name="query" placeholder="π Address 2" target=""><br />
    <input type="text" class="search-box" name="query" placeholder="π? Postcode" target="">
    <br /><br /><br />
    <h6><b style="font-weight:400;"><i class="fas fa-phone"></i> DIETARY REQUIREMENTS / ι»θ©±ηͺε·</b></h6>
    <select name="allergies" id="allergies" class="search-box" target="" onchange="dropdownChange();">
      <option value="none">π² No Allergy Requirements</option>
      <option value="nuts">Nuts</option>
      <option value="crustacean">Crustacean</option>
      <option value="lactose">Lactose</option>
      <option value="eggs">Eggs</option>
      <option value="wheat">Wheat</option>
      <option value="gluten">Gluten</option>
      <option value="soy">Soy</option>
      <option value="fish">Fish</option>
      <option value="other">Other</option>
    </select>
    <br />
    <select name="dietary" id="dietary" class="search-box" target="" onchange="dropdownChange();">
      <option value="none">π² No Dietary Requirements</option>
      <option value="vegetarian">π Vegetarian</option>
      <option value="vegan">π Vegan</option>
      <option value="halal">βͺ Halal</option>
      <option value="kosher">β‘ Kosher</option>
      <option value="other">Other</option>
    </select>
    <button type="submit"><i class="fas fa-arrow-right"></i></button>
      <!-- <input type="submit" value="π" id="search-button"> -->
    </form>
    <br /><br />

  <p>
    <a class="btn btn-primary" data-toggle="collapse" href="#multiCollapseExample1" role="button" aria-expanded="false" aria-controls="multiCollapseExample1">Click if "Other"</a>
  </p>
  <div class="row">
    <div class="col">
      <div class="collapse multi-collapse" id="multiCollapseExample1">
        <div class="card card-body">
          <h4>Click the submit button above, if "Other" has been chosen.</h4>
          <input type="text" class="search-box" id="other-allergies" name="query" placeholder="π² Other Allergies" target="">
          <br />
          <input type="text" class="search-box" id="other-dietary" name="query" placeholder="π² Other Dietary Requirements" target="">
        </div>
      </div>
    </div>
  </div>


  <br /><br /><br />
  <h6><b style="font-weight:400;"><i class="fab fa-spotify"></i> SPOTIFY INTEGRATIONγ»</b></h6>
  Integrate your Spotify account.<br /><br />
  <form action="{{ site.baseurl }}/spotify_search.html" method="get" id="search-ui">
    <!-- <label for="search-box">Search: </label> -->
    <h5><i class="fab fa-spotify"></i><b> Log In with Spotify</b></h5>
    <i class="fas fa-user"></i> <input type="text" class="search-box" name="query" placeholder="πΆ Spotify Username" target="">
    <br />
    <i class="fas fa-unlock"></i> <input type="password" class="search-box" name="query" placeholder="πΆ Spotify Password"  target="">
    <br /><br /><br />
    <i class="fas fa-search"></i> <input type="number" class="search-box" name="query" placeholder="π Search Song..." target="">
    <button type="submit">
      <i class="fab fa-spotify"></i>
    </button>
    <!-- <input type="submit" value="π" id="search-button"> -->
  </form>
</div>
<br /><br />

---