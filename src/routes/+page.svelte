<script>
  import Card from "../components/Card.svelte";
  import Footer from "../components/Footer.svelte";
  import HomePage from "../components/HomePage.svelte";
  import Logo from "../components/Logo.svelte";
  import Navbar from "../components/Navbar.svelte";

  import apple from '$lib/image/apple.png';
  import adobe from '$lib/image/adobe.png';
  import slack from '$lib/image/slack.png';
  import spotify from '$lib/image/spotify.png';
  import google from '$lib/image/google.png';

  import Aisyah from '$lib/image/Aisyah.png';
  import Angga from '$lib/image/Angga.png';
  import Mabdul from '$lib/image/Mabdul.png';
  import Wo_You from '$lib/image/Wo You.png';

</script>

<main class="bg-stone-200 scroll-smooth">
  <div>
    <Navbar></Navbar>
    <HomePage></HomePage>

    <div class="text text-center">
      <h3 class="mt-16 mb-7 font-medium text-base">Trusted by Global Companies</h3>
      <div class="logo flex flex-wrap justify-center gap-20 md:flex-wrap">
        <Logo imageSrc="{apple}"/>
        <Logo imageSrc="{adobe}"/>
        <Logo imageSrc="{slack}"/>
        <Logo imageSrc="{spotify}"/>
        <Logo imageSrc="{google}"/>
      </div>
    </div>
    
    <div class="card-pic flex flex-col items-center justify-center min-h-screen mt-12 mb-8">
      <div class="name text-center mb-14">
        <h3 class="font-medium text-lg">Grow Today</h3>
        <h1 class="font-semibold text-3xl">Start Your Career</h1>
      </div>
    
      <div class="card grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-4 justify-center">
        <Card
          imageSrc="{Aisyah}"
          title="Aisyah"
          description="I teach how to start UX."
        />
    
        <Card
          imageSrc="{Angga}"
          title="Angga"
          description="I teach how to design tests."
        />
    
        <Card
          imageSrc="{Mabdul}"
          title="Mabdul"
          description="I teach how to assess designs."
        />
    
        <Card
          imageSrc="{Wo_You}"
          title="Wo You"
          description="I teach how to create icons."
        />
      </div>
    </div>

    <Footer></Footer>
    
    <style>
      @import url('https://fonts.googleapis.com/css2?family=Poppins&display=swap');

      html{
        scroll-behavior: smooth;
      }
      main {
          font-family: 'Poppins', sans-serif;
      }
  </style>

  </div>

</main>