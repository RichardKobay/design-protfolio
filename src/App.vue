<template>
  <div class="banner-1">
    <!-- NavBar -->
    <nav
      class="container px-6 mx-auto md:flex md:justify-between md:items-center"
    >
      <div class="flex items-center justify-between">
        <div class="relative w-16 h-16 overflow-hidden">
          <img
            class="overflow-hidden border border-gray-100 rounded-full shadow-sm over"
            src="./assets/yo-cortado.jpg"
            alt="user image"
          />
        </div>
        <!-- Mobile menu button -->
        <div @click="showMenu = !showMenu" class="flex md:hidden">
          <button
            type="button"
            class="text-gray-800 hover:text-gray-400 focus:outline-none focus:text-gray-400"
          >
            <svg viewBox="0 0 24 24" class="w-6 h-6 fill-current">
              <path
                fill-rule="evenodd"
                d="M4 5h16a1 1 0 0 1 0 2H4a1 1 0 1 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2z"
              ></path>
            </svg>
          </button>
        </div>
      </div>
      <!-- Mobile Menu open: "block", Menu closed: "hidden" -->
      <ul
        :class="showMenu ? 'flex' : 'hidden'"
        class="flex-col items-end mt-8 space-y-4 md:flex md:space-y-0 md:flex-row md:items-center md:space-x-10 md:mt-0"
      >
        <li class="menu-button"><a href="#">Home</a></li>
        <li class="menu-button"><a href="#work" v-smooth-scroll>Works</a></li>
        <li class="menu-button">
          <a href="#testimonial" v-smooth-scroll>Testimonials</a>
        </li>
        <li class="menu-button"><a href="#about" v-smooth-scroll>About</a></li>
      </ul>
    </nav>
    <!-- End Navbar -->

    <div class="flex items-center">
      <div class="w-11/12 space-y-5 md:space-y-10">
        <h3
          class="px-2 py-1 text-sm font-semibold text-gray-700 rounded-lg hello-button w-fit md:py-3 md:px-5 3xl:text-3xl 2xl:text-xl lg:text-xl md:text-md font-work_sans"
        >
          👋 Hola,
        </h3>
        <h1
          class="text-xl font-bold leading-tight text-gray-700 3xl:text-8xl 2xl:text-7xl xl:text-6xl lg:text-4xl md:text-3xl sm:text-3xl font-Eczar"
        >
          It's
          <a
            href="https://github.com/richardKobay/"
            target="_blank"
            class="text-black hover:underline"
          >
            RichardKobay</a
          >🙇‍♀️<br />Creative Designer and Storyteller (also a great developer)
        </h1>

        <div class="gap-1 md:flex md:gap-10">
          <a href="#work" v-smooth-scroll>
            <button class="hidden text-white bg-gray-800 submit-button md:block">
              View My Work
            </button>
          </a>
          <a href="#about" v-smooth-scroll>
            <button
              class="mb-5 text-gray-800 border-4 border-gray-800 submit-button md:mb-0"
            >
              Contact Me
            </button>
          </a>
        </div>
      </div>

      <div class="flex justify-end w-8/12">
        <img
          class="3xl:h-[800px] 2xl:h-[650px] xl:h-[550px] lg:h-[550px] md:h-[450px] sm:h-[350px]"
          src="./assets/profile-female.png"
          alt="user image"
        />
      </div>
    </div>
  </div>

  <div class="pb-20 space-y-10 banner-2" id="work">
    <h3 class="my-5 heading3">My Recent Work</h3>
    <div class="card">
      <div class="px-8 py-8 space-y-5 md:py-16 md:px-20 md:w-1/2">
        <h4 class="project-title item">Plantitas</h4>
        <p class="pr-12 font-work_sans">
          Designed an app that helps people to take care of their plants. The
          app is designed in a way that it helps the user to take care of their
          plants.
        </p>
        <a href="https://docs.google.com/presentation/d/1wofcKQVYe3TVz9ow21pUr4rNN8zosNV-e4j7YNEJz-M/edit#slide=id.p">
          <button class="text-2xl font-bold tracking-wider text-sky-800">
            View Case Study
          </button>
        </a>
        <a href="https://www.figma.com/proto/Eg5PPs5eGZSGBRIL0GqtkU/plantitas?page-id=0%3A1&node-id=1103-96&p=f&viewport=609%2C439%2C0.49&t=icCIfWuLaYoePEbe-1&scaling=min-zoom&content-scaling=fixed">
          <button class="text-2xl font-bold tracking-wider text-sky-800">
            View Mobile prototype
          </button>
        </a>
      </div>
      <div class="bg-green-100 card-image">
        <img
          class="object-cover w-full h-72 md:h-96"
          src="./assets/plantitas.png"
        />
      </div>
    </div>

    <div class="card">
      <div class="px-8 py-8 space-y-5 md:py-16 md:px-20 md:w-1/2">
        <h4 class="project-title item">Nutricionsita</h4>
        <p class="pr-12 font-work_sans">
          Designed an app that helps people to take care of their nutrition. The
          app is designed in a way that it helps the user to take care of their
          health and nutrition. The app is useful and easy to use, not to mention that is pretty beautiful.
        </p>
        <a href="https://www.figma.com/deck/WRFv2MXUkmrgjfHhN6B9e3/Nutricionsita---Slides?node-id=1-42&viewport=-34%2C-96%2C0.47&t=IIltKJjogp41ptM5-1&scaling=min-zoom&content-scaling=fixed&page-id=0%3A1">
          <button class="text-2xl font-bold tracking-wider text-sky-800">
            View Case Study
          </button>
        </a>
        <a href="https://www.figma.com/proto/NBTCI0xRkkLk6CuRENsSBj/Nutricioncita?page-id=0%3A1&node-id=3-69&p=f&viewport=231%2C260%2C0.23&t=tcWjKEWRqoaFgeIR-1&scaling=min-zoom&content-scaling=fixed&starting-point-node-id=3%3A69&show-proto-sidebar=1">
          <button class="text-2xl font-bold tracking-wider text-sky-800">
            View Mobile prototype
          </button>
        </a>
      </div>
      <div class="card-image">
        <img
          class="object-cover w-full h-48 md:h-96"
          src="./assets/nutricionsita.png"
        />
      </div>
    </div>
  </div>

  <div class="banner-1" id="testimonial">
    <div class="grid mt-5 space-y-4 place-items-center">
      <h3 class="heading3">Some Generous Words</h3>
      <p class="font-semibold leading-relaxed text-gray-600 font-work_sans">
        Some of my favorite testimonials from my clients
      </p>
    </div>
    <div class="max-w-6xl px-8 py-16 mx-auto">
      <div class="relative">
        <div class="relative overflow-hidden rounded-lg shadow-2xl lg:flex">
          <div
            class="relative flex items-center justify-center h-56 lg:h-auto lg:w-5/12"
          >
            <img
              class="absolute object-cover w-full h-full"
              src="./assets/cubosls-logo.png"
              alt=""
            />
            <div class="absolute inset-0 bg-gray-700 opacity-75"></div>
          </div>
          <div class="relative bg-white lg:w-7/12">
            <svg
              class="absolute w-24 h-full -ml-12 text-white"
              fill="currentColor"
              viewBox="0 0 100 100"
              preserveAspectRatio="none"
            >
              <polygon points="50,0 100,0 50,100 0,100" />
            </svg>
            <div
              class="relative px-8 py-12 leading-relaxed text-gray-700 lg:py-24 lg:px-16"
            >
              <h2 class="text-5xl font-bold">CUBOS LS</h2>
              <p>
                As
                <strong class="font-medium text-gray-900">Cubos LS</strong> grows
                rapidly, working with RichardKobay is pretty much like working with
                a friend. He is always there to help and support us.
              </p>
              <p class="mt-6">
                <a
                  href="http://cubosls.com/"
                  class="font-medium text-indigo-600 hover:text-indigo-900"
                >
                  &rarr; Md Solaiman Hossain</a
                >
              </p>
            </div>
          </div>
        </div>
        <div class="absolute inset-y-0 left-0 lg:flex lg:items-center">
          <button
            class="w-12 h-12 p-3 mt-24 -ml-6 bg-white rounded-full shadow-lg lg:mt-0"
          >
            <svg
              class="w-full h-full text-indigo-900"
              fill="currentColor"
              viewBox="0 0 24 24"
            >
              <path
                d="M5.41 11H21a1 1 0 0 1 0 2H5.41l5.3 5.3a1 1 0 0 1-1.42 1.4l-7-7a1 1 0 0 1 0-1.4l7-7a1 1 0 0 1 1.42 1.4L5.4 11z"
              />
            </svg>
          </button>
        </div>
        <div class="absolute inset-y-0 right-0 lg:flex lg:items-center">
          <button
            class="w-12 h-12 p-3 mt-24 -mr-6 bg-white rounded-full shadow-lg lg:mt-0"
          >
            <svg
              class="w-full h-full text-indigo-900"
              fill="currentColor"
              viewBox="0 0 24 24"
            >
              <path
                d="M18.59 13H3a1 1 0 0 1 0-2h15.59l-5.3-5.3a1 1 0 1 1 1.42-1.4l7 7a1 1 0 0 1 0 1.4l-7 7a1 1 0 0 1-1.42-1.4l5.3-5.3z"
              />
            </svg>
          </button>
        </div>
      </div>
    </div>
  </div>

  <div class="items-center banner-2 md:flex md:justify-evenly" id="about">
    <img
      class="md:h-[500px] h-[400px]"
      src="./assets/about-female.png"
      alt="user image"
    />
    <div class="px-8 py-8 space-y-5 md:py-16 md:px-20 md:w-1/2">
      <h4 class="project-title item">About Me</h4>
      <p class="font-work_sans">
        I am RichardKobay (Ricardo Soriano), a designer and storyteller. I am a
        designer who loves to create beautiful and functional designs. I like anime
        and develop beautiful things.
      </p>
      <a href="https://drive.google.com/file/d/1k9PexYY_mm8FS8lcV5-I9UchvizJgOHo/view?usp=sharing" download>
        <button class="text-2xl font-bold tracking-wider text-sky-800">
          Download my CV
        </button>
      </a>
    </div>
  </div>

  <div class="flex items-center h-full banner-1">
    <div class="w-7/12 p-12">
      <h2 class="mb-5 text-2xl font-bold text-gray-700 md:text-6xl font-Eczar">
        Let’s work together and make everything super cute and super useful.
      </h2>
      <a class="text-2xl text-blue-600 underline font-work_sans" href="mailto:ricardo.roel110@gmail.com"
        >📧 ricardo.roel110@gmail.com</a
      >
    </div>
    <div class="w-5/12 pr-28">
      <div class="flex flex-wrap justify-end gap-2">
        <a href="https://www.facebook.com/ricardo.roel.98">
          <button
            class="inline-flex items-center p-2 space-x-2 font-semibold text-white bg-gray-700 rounded"
          >
            <svg
              class="w-4 h-4 fill-current md:w-10 md:h-10 lg:w-10 lg:h-10 xl:h-10 xl:w-10"
              role="img"
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 24 24"
            >
              <path
                d="M24 12.073c0-6.627-5.373-12-12-12s-12 5.373-12 12c0 5.99 4.388 10.954 10.125 11.854v-8.385H7.078v-3.47h3.047V9.43c0-3.007 1.792-4.669 4.533-4.669 1.312 0 2.686.235 2.686.235v2.953H15.83c-1.491 0-1.956.925-1.956 1.874v2.25h3.328l-.532 3.47h-2.796v8.385C19.612 23.027 24 18.062 24 12.073z"
              />
            </svg>
          </button>
        </a>

        <a href="https://x.com/RichardKobay">
          <button
            class="inline-flex items-center p-2 space-x-2 font-semibold text-white bg-gray-700 rounded"
          >
            <svg
              class="w-4 h-4 fill-current md:w-10 md:h-10 lg:w-10 lg:h-10 xl:h-10 xl:w-10"
              role="img"
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 24 24"
            >
              <path
                d="M23.953 4.57a10 10 0 01-2.825.775 4.958 4.958 0 002.163-2.723c-.951.555-2.005.959-3.127 1.184a4.92 4.92 0 00-8.384 4.482C7.69 8.095 4.067 6.13 1.64 3.162a4.822 4.822 0 00-.666 2.475c0 1.71.87 3.213 2.188 4.096a4.904 4.904 0 01-2.228-.616v.06a4.923 4.923 0 003.946 4.827 4.996 4.996 0 01-2.212.085 4.936 4.936 0 004.604 3.417 9.867 9.867 0 01-6.102 2.105c-.39 0-.779-.023-1.17-.067a13.995 13.995 0 007.557 2.209c9.053 0 13.998-7.496 13.998-13.985 0-.21 0-.42-.015-.63A9.935 9.935 0 0024 4.59z"
              />
            </svg>
          </button>
        </a>

        <button
          class="inline-flex items-center p-2 space-x-2 font-semibold text-white bg-gray-700 rounded"
        >
          <svg
            class="w-4 h-4 fill-current md:w-10 md:h-10 lg:w-10 lg:h-10 xl:h-10 xl:w-10"
            role="img"
            viewBox="0 0 24 24"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M12 0A12 12 0 0 0 0 12a12 12 0 0 0 12 12 12 12 0 0 0 12-12A12 12 0 0 0 12 0zm5.01 4.744c.688 0 1.25.561 1.25 1.249a1.25 1.25 0 0 1-2.498.056l-2.597-.547-.8 3.747c1.824.07 3.48.632 4.674 1.488.308-.309.73-.491 1.207-.491.968 0 1.754.786 1.754 1.754 0 .716-.435 1.333-1.01 1.614a3.111 3.111 0 0 1 .042.52c0 2.694-3.13 4.87-7.004 4.87-3.874 0-7.004-2.176-7.004-4.87 0-.183.015-.366.043-.534A1.748 1.748 0 0 1 4.028 12c0-.968.786-1.754 1.754-1.754.463 0 .898.196 1.207.49 1.207-.883 2.878-1.43 4.744-1.487l.885-4.182a.342.342 0 0 1 .14-.197.35.35 0 0 1 .238-.042l2.906.617a1.214 1.214 0 0 1 1.108-.701zM9.25 12C8.561 12 8 12.562 8 13.25c0 .687.561 1.248 1.25 1.248.687 0 1.248-.561 1.248-1.249 0-.688-.561-1.249-1.249-1.249zm5.5 0c-.687 0-1.248.561-1.248 1.25 0 .687.561 1.248 1.249 1.248.688 0 1.249-.561 1.249-1.249 0-.687-.562-1.249-1.25-1.249zm-5.466 3.99a.327.327 0 0 0-.231.094.33.33 0 0 0 0 .463c.842.842 2.484.913 2.961.913.477 0 2.105-.056 2.961-.913a.361.361 0 0 0 .029-.463.33.33 0 0 0-.464 0c-.547.533-1.684.73-2.512.73-.828 0-1.979-.196-2.512-.73a.326.326 0 0 0-.232-.095z"
            />
          </svg>
        </button>

        <button
          class="inline-flex items-center p-2 space-x-2 font-semibold text-white bg-gray-700 rounded"
        >
          <svg
            class="w-4 h-4 fill-current md:w-10 md:h-10 lg:w-10 lg:h-10 xl:h-10 xl:w-10"
            role="img"
            viewBox="0 0 24 24"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M12.017 0C5.396 0 .029 5.367.029 11.987c0 5.079 3.158 9.417 7.618 11.162-.105-.949-.199-2.403.041-3.439.219-.937 1.406-5.957 1.406-5.957s-.359-.72-.359-1.781c0-1.663.967-2.911 2.168-2.911 1.024 0 1.518.769 1.518 1.688 0 1.029-.653 2.567-.992 3.992-.285 1.193.6 2.165 1.775 2.165 2.128 0 3.768-2.245 3.768-5.487 0-2.861-2.063-4.869-5.008-4.869-3.41 0-5.409 2.562-5.409 5.199 0 1.033.394 2.143.889 2.741.099.12.112.225.085.345-.09.375-.293 1.199-.334 1.363-.053.225-.172.271-.401.165-1.495-.69-2.433-2.878-2.433-4.646 0-3.776 2.748-7.252 7.92-7.252 4.158 0 7.392 2.967 7.392 6.923 0 4.135-2.607 7.462-6.233 7.462-1.214 0-2.354-.629-2.758-1.379l-.749 2.848c-.269 1.045-1.004 2.352-1.498 3.146 1.123.345 2.306.535 3.55.535 6.607 0 11.985-5.365 11.985-11.987C23.97 5.39 18.592.026 11.985.026L12.017 0z"
            />
          </svg>
        </button>

        <a href="https://www.linkedin.com/in/juan-ricardo-soriano-roel-78514321b/">
          <button
            class="inline-flex items-center p-2 space-x-2 font-semibold text-white bg-gray-700 rounded"
          >
            <svg
              class="w-4 h-4 fill-current md:w-10 md:h-10 lg:w-10 lg:h-10 xl:h-10 xl:w-10"
              role="img"
              viewBox="0 0 256 256"
              xmlns="http://www.w3.org/2000/svg"
            >
              <g>
                <path
                  d="M218.123122,218.127392 L180.191928,218.127392 L180.191928,158.724263 C180.191928,144.559023 179.939053,126.323993 160.463756,126.323993 C140.707926,126.323993 137.685284,141.757585 137.685284,157.692986 L137.685284,218.123441 L99.7540894,218.123441 L99.7540894,95.9665207 L136.168036,95.9665207 L136.168036,112.660562 L136.677736,112.660562 C144.102746,99.9650027 157.908637,92.3824528 172.605689,92.9280076 C211.050535,92.9280076 218.138927,118.216023 218.138927,151.114151 L218.123122,218.127392 Z M56.9550587,79.2685282 C44.7981969,79.2707099 34.9413443,69.4171797 34.9391618,57.260052 C34.93698,45.1029244 44.7902948,35.2458562 56.9471566,35.2436736 C69.1040185,35.2414916 78.9608713,45.0950217 78.963054,57.2521493 C78.9641017,63.090208 76.6459976,68.6895714 72.5186979,72.8184433 C68.3913982,76.9473153 62.7929898,79.26748 56.9550587,79.2685282 M75.9206558,218.127392 L37.94995,218.127392 L37.94995,95.9665207 L75.9206558,95.9665207 L75.9206558,218.127392 Z M237.033403,0.0182577091 L18.8895249,0.0182577091 C8.57959469,-0.0980923971 0.124827038,8.16056231 -0.001,18.4706066 L-0.001,237.524091 C0.120519052,247.839103 8.57460631,256.105934 18.8895249,255.9977 L237.033403,255.9977 C247.368728,256.125818 255.855922,247.859464 255.999,237.524091 L255.999,18.4548016 C255.851624,8.12438979 247.363742,-0.133792868 237.033403,0.000790807055"
                ></path>
              </g>
            </svg>
          </button>
        </a>
      </div>
    </div>
  </div>
</template>
<script>
  export default {
    data() {
      return {
        showMenu: false,
      }
    },
  }
</script>
