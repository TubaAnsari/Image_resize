<script>
  // javascript code
</script>

<!-- ================================================= -->

<!-- for use backgroud color -->
<div class="background-container">
  <!-- Your content goes here -->
  <slot />

  <!-- for Heading container Box  -->
  <center>
    <div class="Heading_container">
      <center>
        <h2>Bulk Resize Images</h2>
      </center>
    </div>

    <!-- for get a padding  -->
    <br /><br />
    <br /><br />
    <br /><br />
  </center>
  <div class="mid">
    <center>
      <div class="mid1">
        
        <div class="properties">

          <br />
          <button type="button" class="bn">Percentage</button>
          <br />
          <button type="button" class="bn">File Size</button>
          <br />
        </div>
      </div>
    </center>
    <div class="mid2">
      <!-- for show a some features in website -->
      <div class="horizontal">
        <h4>Percentage</h4>
        Scale images to &nbsp
        <input
          type="text"
          class="form-control Centered-Input"
          value="50"
          style="width: 70px; display: inline;"
        />
        &nbsp % of the original dimensions.
      </div>
      <br />
      <div class="horizontal1">
        <h4>Image Format</h4>
        <div class="dropdown">
          <button class="dropbtn">JPEG</button>
          <div class="dropdown-content">
            <!-- svelte-ignore a11y-missing-attribute -->
            <a >JPEG</a>
            <!-- svelte-ignore a11y-missing-attribute -->
            <a >PNG</a>
            <!-- svelte-ignore a11y-missing-attribute -->
            <a >WEBP</a>
          </div>
        </div>
      </div>

      <div class="horizontal2">
        <h4>Image Quality</h4>
        <input
          class="form-control-range"
          type="range"
          min="0.25"
          max="1"
          step="0.01"
          value="0.79"
        />
        <div style="text-align: center; color: #181717;">79%</div>
        
      </div>
    </div>
  </div>
</div>

<!-- CSS style section -->

<style>
    .background-container {
      width: 100%;
      height: 100%;
      background-size: cover;
      position: fixed;
      background-color: #e4e5e6;
      background-repeat: no-repeat;
      background-attachment: fixed;
      opacity: 70%;
      z-index: -1;
      /* text-align: start; */
    } 
  .mid {
    flex-flow: wrap;
  }
  /* heading Style */
  .Heading_container {
    /* border: 2px solid red; */
    height: 40opx;
    width: 400px;

    display: flex;
    justify-content: center;
    align-items: center;
    align-content: flex-end;
    background-color: #aebdca;
    border-radius: 8px;
    /* box-shadow: 0px 20px 50px grey  ; */
    box-shadow: 0 8px 6px -6px rgb(36, 35, 35);
    /* object-fit: ; */
  }
  h2 {
    font-size: 30px;
  }

  /* drop image container style */
  .properties {
    height: 200px;
    width: 1200px;
    background-color: #aebdca;
    border-radius: 8px;
    box-shadow: 0 8px 6px -6px rgb(36, 35, 35);
    align-content: center;
    justify-content: center;
    align-items: center;
    font-size: 28px;
    padding-top: 1%;
  }

  /* choose button style */
  .bn {
    height: 30%;
    width: 50%;
    font-size: medium;
    color: white;
    font-weight: 700;

    display: flex;
    justify-content: center;
    align-items: center;
    padding: 10px;
    gap: 10px;
    margin-left: 50px;
    background-color: #181717;
    outline: 3px #181717 solid;
    outline-offset: -3px;
    border-radius: 5px;
    border: none;
    cursor: pointer;
    transition: 400ms;
  }

  /* website features style */
  .horizontal {
    display: inline-block;
    padding-top: 7%;
    padding-left: 12%;
  }
  .horizontal1 {
    display: inline-block;
    padding-top: 3%;
    padding-left: 12%;
  }
  .dropdown {
    position: relative;
    display: inline-block;
  }

  /* Style for the button that triggers the dropdown */
  .dropbtn {
    background-color: #181717;
    color: white;
    padding: 10px 20px;
    border: none;
    cursor: pointer;
    border-radius: 7px;
  }

  /* Style for the dropdown content (hidden by default) */
  .dropdown-content {
    display: none;
    position: absolute;
    background-color: #f9f9f9;
    min-width: 160px;
    box-shadow: 0px 8px 16px 0px rgba(0, 0, 0, 0.2);
    z-index: 1;
  }

  /* Style for the individual dropdown items */
  .dropdown-content a {
    padding: 12px 16px;
    text-decoration: none;
    display: block;
    color: #333;
  }

  /* Change color on hover */
  .dropdown-content a:hover {
    background-color: #ddd;
  }

  /* Show the dropdown when the button is hovered over */
  .dropdown:hover .dropdown-content {
    display: block;
  }

  .horizontal2 {
    display: inline-block;
    padding-top: 3%;
    padding-left: 12%;
  }

</style>
