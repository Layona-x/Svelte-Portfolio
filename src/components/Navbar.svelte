<script>
  let nav = { navOpen:false }
	function navClick() {
		 nav.navOpen = !nav.navOpen;
    console.log(nav)
  }
</script>
<nav class="navbar">
    <div class="navbar-brand__items">
     <div style="height:50px;display:flex;justify-content: space-between">
    <h1>Layona</h1>
    <button on:click={navClick} class="navbar-brand__button"><i class="fa-solid fa-bars"></i></button>
     </div>
    </div> 
   {#if nav.navOpen}
  <div class="navbar-brand">
        <a href="#home"><li style="margin-top:15px" class="extend-item"><p>Home</p></li></a><hr>
        <a href="#about"><li class="extend-item"><p>About Me?</p></li></a><hr>
        <a href="#developers"> <li class="extend-item"><p>Developer Skills</p></li></a><hr>
        <a href="#contact"><li class="extend-item"><p>Contact Me</p></li></a><hr>
        <a><li class="extend-item"><p>Blogs</p></li><br></a>
  </div>
  {/if}
</nav>


<br><br>
