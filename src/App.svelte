<script>
  import "./app.css";
  let showImage = true;
  let showImage0 = true;
</script>

<main class="relative bg-gray-900">
  <section class="text-gray-600 -mt-20 body-font mb-20">
    <div class="text-center w-full mb-12">
      <h1 class="sm:text-3xl text-2xl font-extrabold title-font mb-4 text-gold">
        Meet the team
      </h1>
    </div>
    <div
      class="mx-10 flex flex-col md:flex-row justify-center text-center items-center"
    >
      <!-- svelte-ignore a11y-mouse-events-have-key-events -->
      <!-- svelte-ignore a11y-click-events-have-key-events -->
      <div
        class="p-2 mb-5 mx-5 text-center bg-transparent rounded-xl border border-white w-full md:w-1/3"
        on:click|preventDefault={() => {
          showImage = !showImage;
        }}
      >
        {#if showImage}
          <div class="lg:mx-[40px] flex justify-center">
            <img
              src="https://slimecars.com/assets/ayden.png"
              alt="founder Ayden Owens-Delerme"
            />
          </div>
        {:else}
          <p class="relative text-left my-[20px] text-gray-200">
            Ayden is a former Arkansas student-athlete, 3x NCAA champion, and a
            World Championship competitor in track and field with a highly
            monetized NIL portfolio. He possesses a Bachelor's degree from the
            University of Michigan and a Master’s in Business Administration
            with a focus in Entrepreneurship from the Sam M. Walton College of
            Business at the University of Arkansas.<br /><br /> Leveraging his unique
            experience in college athletics before and after NIL’s legalization,
            Ayden was driven to create DapUp to eliminate the friction and ambiguity
            around brand-athlete partnerships. Ayden’s passion lies at the intersection
            of business and sport, where two industries join to drive the world forward.
            He is also invested in social justice and promoting sports opportunities
            to underserved communities by providing coaching services for youth athletes.
            Ayden’s mission is to create an equitable and more accessible market
            for NIL allowing all businesses and athletes to benefit.
          </p>
        {/if}
        <p class="text-lg text-white">Ayden Owens-Delerme, MBA</p>
        <p class="text-sm text-white">
          Founder & Chief Executive Officer <br /> 3x NCAA Champion
        </p>
        <p
          class="text-[15px] hidden md:block text-right text-gray-500"
          style="transform: translateY(9px)"
        >
          click for more info >
        </p>
        <p
          class="text-[15px] lg:hidden md:hidden text-right text-gray-500"
          style="transform: translateY(9px)"
        >
          tap for more info
        </p>
      </div>
      <div
        class="p-2 mb-5 mx-5 text-center bg-transparent rounded-xl border border-white w-full md:w-1/3"
        on:click|preventDefault={() => {
          showImage0 = !showImage0;
        }}
      >
        {#if showImage0}
          <div class=" lg:mx-[40px] flex justify-center">
            <img
              src="https://slimecars.com/assets/quintin.jpg"
              alt="founder quintin owens"
            />
          </div>
        {:else}
          <p class="text-left relative h-full my-[102px] text-gray-200">
            Quintin is an entrepreneur, former athlete, and a sales professional
            at SAE International. He holds a breadth of experience in
            understanding the needs of companies worldwide as he ensures they
            are suited with up-to-date standards for business operation.<br
            /><br /> As a small business operator and founder of an apparel company,
            Quintin was drawn to DapUp for the impact it has on helping brands like
            his reach the right audience. His objective is to promote the growth
            of businesses at all levels through the DapUp platform.
          </p>
        {/if}
        <p class="text-lg text-white">Quintin Owens</p>
        <p class="text-sm text-white">Chief Sales Officer<br /><br /></p>
        <p
          class="text-[15px] hidden md:block text-right text-gray-500"
          style="transform: translateY(9px)"
        >
          click for more info >
        </p>
        <p
          class="text-[15px] lg:hidden md:hidden text-right text-gray-500"
          style="transform: translateY(9px)"
        >
          tap for more info
        </p>
      </div>
    </div>
  </section>
</main>

<style>
  .logo {
    height: 6em;
    padding: 1.5em;
    will-change: filter;
    transition: filter 300ms;
  }
  .logo:hover {
    filter: drop-shadow(0 0 2em #646cffaa);
  }
  .logo.svelte:hover {
    filter: drop-shadow(0 0 2em #ff3e00aa);
  }
  .read-the-docs {
    color: #888;
  }
</style>
