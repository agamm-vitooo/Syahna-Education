<script>
  export let imageSrc = ".image/";
  export let title = "Judul Card";
  export let description = "Deskripsi card yang singkat.";
  
</script>

<div class="container min-h-full text-center w-fit">
  <div class="card">
    <div class="card-1 flex flex-wrap">
      <div class="max-w-xs bg-white rounded-2xl overflow-hidden">
        <img src={imageSrc} alt="Gambar Card" class="w-full" />
        <div class="px-6 py-4">
          <div class="font-medium text-xl mb-2 text-left">{title}</div>
          <p class="text-stone-500 font-light text-base text-left">{description}</p>
        </div>
      </div>
    </div>
  </div>
</div>