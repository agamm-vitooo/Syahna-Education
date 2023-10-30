<script>
  import hero from '$lib/image/hero.png';
  import star from '$lib/image/Star.png';
  import pattern from '$lib/image/pattern.png';
  import circle from '$lib/image/circle.png';
</script>

<div class="container px-10 sm:px-28 relative">
  <div class="pattern-background">
    <img src={pattern} alt="pattern" class="absolute inset-0 w-full h-full object-cover z-0">
  </div>
  <div class="min-h-screen bg-transparent text-white py-10 px-4 md:flex md:justify-between md:items-center justify-around">
    <div class="title md:w-1/2 mb-4 md:mb-0 relative z-20">
      <h1 class="text-5xl font-semibold text-black mb-7">Learn UI Design <br>
        From The Real Expert</h1>
      <p class="text-base font-thin text-stone-400">Stop wasting time browsing around and start learning <br>
        from our designers for your better career.</p>
      <button class="bg-green-500 py-2 px-4 rounded-md text-black mt-12 hover:bg-green-400">Get Started</button>
    </div>
    <div class="relative md:w-1/2">
      <img src={circle} alt="circle" class="absolute top-0 right-0 sm:top-44 sm:right-28 w-16 h-auto">
      <img src={hero} alt="Hero" class="w-50 h-auto" />
      <span class="absolute bottom-0 left-1/2 -translate-x-1/2 md:scale-125">
        <div class="w-[180px] h-[130px] relative right-10 sm:right-44 top-16 sm:top-0">
          <div class="w-[180px] h-[130px] left-0 top-0 absolute bg-white rounded-[20px]"></div>
          <div class="left-[20px] top-[20px] absolute text-neutral-800 text-base font-medium font-['Poppins']">Corellina Xo</div>
          <div class="left-[20px] top-[46px] absolute text-stone-400 text-sm font-light font-['Poppins']">UI Designer</div>
          <div class="relative flex items-center top-20 left-3">
            <img src={star} alt="Star" class="w-6 h-6">
            <img src={star} alt="Star" class="w-6 h-6">
            <img src={star} alt="Star" class="w-6 h-6">
            <img src={star} alt="Star" class="w-6 h-6">
            <img src={star} alt="Star" class="w-6 h-6">
          </div>
        </div>
      </span>
    </div>
  </div>
</div>

<style>
  
</style>

