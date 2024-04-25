<script>
export default {
  data() {
    return {
      activeTab: 1,
      tech: [
        {
          id: 5,
          name: 'Visual Effect',
          imageUrl: 'https://i.ibb.co/sgTNDNL/clapperboard.png',
          status: 'Advance'
        },
        {
          id: 6,
          name: 'Animation',
          imageUrl: 'https://i.ibb.co/9yS7zsH/3d-movie.png',
          status: 'Advance'
        },
        {
          id: 13,
          name: 'Motion Graphic',
          imageUrl: 'https://i.ibb.co/qxXF1wj/motion-graphic.png',
          status: 'Advance'
        },
        {
          id: 7,
          name: 'Graphic Design',
          imageUrl: 'https://i.ibb.co/R76Q3QG/illustration.png',
          status: 'Advance'
        },
        {
          id: 8,
          name: 'Video Editing',
          imageUrl: 'https://i.ibb.co/WKQ9x0X/video.png',
          status: 'Advance'
        },
        {
          id: 9,
          name: 'Product Ads',
          imageUrl: 'https://i.ibb.co/WKQ9x0X/video.png',
          status: 'Advance'
        },
        {
          id: 10,
          name: 'Videography',
          imageUrl: 'https://i.ibb.co/qFdQmWp/camera.png',
          status: 'Advance'
        },
        {
          id: 11,
          name: 'Bootstrap',
          imageUrl: 'https://getbootstrap.com/docs/5.2/assets/brand/bootstrap-logo-shadow.png',
          status: 'Intermediate'
        },
        {
          id: 12,
          name: 'Filmmaking',
          imageUrl: 'https://i.ibb.co/pJX6G1v/video-camera.png',
          status: 'Intermediate'
        },
        {
          id: 1,
          name: 'HTML',
          imageUrl: 'https://cdn-icons-png.flaticon.com/512/1051/1051277.png',
          status: 'Advanced'
        },
        {
          id: 2,
          name: 'CSS',
          imageUrl: 'https://cdn-icons-png.flaticon.com/512/732/732190.png',
          status: 'Advanced'
        },
        {
          id: 3,
          name: 'PHP',
          imageUrl: 'https://cdn.iconscout.com/icon/free/png-256/free-php-2038871-1720084.png',
          status: 'Advanced'
        },
        {
          id: 4,
          name: 'Javascript',
          imageUrl: 'https://cdn.icon-icons.com/icons2/2415/PNG/512/javascript_original_logo_icon_146455.png',
          status: 'Advance'
        },
      ],
      tools: [
        {
          id: 1,
          name: 'Illustrator',
          imageUrl: 'https://i.ibb.co/dLPX8Fn/illustrator.png',
          status: '2D Animation'
        },
        {
          id: 2,
          name: 'Adobe',
          imageUrl: 'https://i.ibb.co/68T3PrR/icons8-adobe-64.png',
          status: 'All Adobe'
        },
        {
          id: 3,
          name: 'Davinci',
          imageUrl: 'https://i.ibb.co/R9fCyKr/icons8-davinci-resolve-100.png',
          status: 'Video Editing'
        },
        {
          id: 4,
          name: 'D. Marketing',
          imageUrl: 'https://i.ibb.co/qdgfg7g/social-media.png',
          status: 'Social Media'
        },
        {
          id: 5,
          name: 'Blender',
          imageUrl: 'https://i.ibb.co/y4JJwMG/icons8-blender-512.png',
          status: '3D Animation'
        },
        {
          id: 6,
          name: 'Premiere Pro',
          imageUrl: 'https://i.ibb.co/zF98PqQ/premiere-pro.png',
          status: 'Video Editing'
        },
        {
          id: 7,
          name: 'After Effect',
          imageUrl: 'https://i.ibb.co/9HZXfPR/after-effects.png',
          status: 'Visual Effect'
        },
        {
          id: 8,
          name: 'XD',
          imageUrl: 'https://i.ibb.co/sWH1ntL/xd.png',
          status: 'Web Design'
        },
        {
          id: 9,
          name: 'VS Code',
          imageUrl: 'https://i.ibb.co/WtDPcB1/icons8-visual-studio-code-2019-512.png',
          status: 'Coding'
        },
        {
          id: 10,
          name: 'Photoshop',
          imageUrl: 'https://i.ibb.co/jhh7YYS/photoshop.png',
          status: 'Editing Photo'
        },
        {
          id: 11,
          name: 'In Design',
          imageUrl: 'https://i.ibb.co/qrTtQ5d/indesign.png',
          status: 'Design'
        },
        {
          id: 12,
          name: 'Lightroom',
          imageUrl: 'https://i.ibb.co/QJp0tSw/photoshop-lightroom.png',
          status: 'Color Grading'
        },
        {
          id: 12,
          name: 'Git',
          imageUrl: 'https://git-scm.com/images/logos/downloads/Git-Icon-1788C.png',
          status: 'Version Control'
        },
        {
          id: 13,
          name: 'GitHub',
          imageUrl: 'https://cdn-icons-png.flaticon.com/512/25/25231.png',
          status: 'Git Hosting'
        },
        {
          id: 14,
          name: 'NPM',
          imageUrl: 'https://cdn.iconscout.com/icon/free/png-256/free-npm-3-1175132.png',
          status: 'Package Manager'
        },
        {
          id: 15,
          name: 'MySQL',
          imageUrl: 'https://cdn-icons-png.flaticon.com/512/5968/5968313.png',
          status: 'Database'
        },
      ]
    };
  }
}
</script>
<template>
  <div
    class="bg-[#1e1e1f] px-5 py-5 md:px-12 md:py-10 text-left border border-[#383838] rounded-3xl text-amber-50 mx-3 mb-5">
    <article data-page="about">

      <header>
        <div class="text-2xl font-bold text-white mb-5 fadein-bot title-section flex items-center">
          About Me &nbsp;
          <div class="h-[1px] w-32 bg-amber-200 md:w-96 aos-init aos-animate" data-aos="zoom-in-left"
            data-aos-duration="600"></div>
        </div>
      </header>

      <section
        class="text-sm md:text-lg text-justify flex flex-col gap-4 md:flex-row md:gap-8 md:justify-left md:items-center">
        <div class="flex justify-center">
          <img class="w-9/12 rounded-full mb-3 fadein-up"
            src="https://i.ibb.co/Snzyk8Q/Yoo.jpg" alt="Foto">
        </div>
        <div class="md:w-7/12">
          <p class="mb-3 md:mb-7 fadein-left fadeins-1">
            &nbsp; &nbsp; &nbsp; Hi everyone! My name is Afif Eka Saputra. I'm a Multimedia Profesional. I
            have 6 year of experience in Multimedia.
            I really enjoy what I do right now, in my opinion, cMultimedia work is not only a job, but also an art
            art is an explosion
          </p>
          <p class="mb-3 fadein-left fadeins-2">
            &nbsp; &nbsp; &nbsp; My duties are Video Editing, Visual Effects, Logo Creation, Website Design, Website Creation, Product Design, Product Advertisement Creation, and Animation Modeling.
            Additionally, I add a personal touch to your product and ensure that it is eye-catching and attractive
            easy to use.
            My goal is to convey your message and identity in the most creative way. If you are interested in hiring me,
            Please contact the contact listed.
          </p>
        </div>

      </section>

    </article>
  </div>

  <div class="px-5 py-5 md:px-12 md:py-10 text-left text-amber-50 mx-3">
    <article data-page="about">
      <header>
        <div class="text-2xl font-bold text-white mb-5 fadein-bot title-section flex items-center">
          <div class="h-[1px] w-10 bg-amber-200 md:w-20 aos-init aos-animate" data-aos="zoom-in-left"
            data-aos-duration="600"></div>
          &nbsp; Skills
        </div>
      </header>
      <section>
        <div>
          <ul class="flex flex-wrap text-sm font-medium text-center text-gray-500 dark:text-gray-400 mb-5">
            <li class="mr-2">
              <button class="inline-block px-4 py-3 rounded-lg hover:text-white"
                :class="{ 'text-amber-200 bg-amber-200 bg-opacity-10': activeTab === 1 }" @click="activeTab = 1">Tech Stack</button>
            </li>
            <li class="mr-2">
              <button class="inline-block px-4 py-3 rounded-lg hover:text-white"
                :class="{ 'text-amber-200 bg-amber-200 bg-opacity-10': activeTab === 2 }" @click="activeTab = 2">Tools</button>
            </li>
          </ul>
        </div>
        <div v-show="activeTab === 1">
          <div class="grid grid-cols-2 gap-4 pb-32 md:grid-cols-3 md:gap-8 xl:grid-cols-4 xl:gap-10 2xl:gap-12">
            <div v-for="item in tech" :key="item.id">
              <div
                class="item-tech flex cursor-pointer items-center gap-2 rounded border border-amber-200 px-2 py-2 hover:bg-amber-200 hover:bg-opacity-10 md:gap-3 lg:px-3">
                <div class="flex h-12 w-12 items-center justify-center p-0 lg:h-16 lg:w-16 lg:p-2 zoom-in">
                  <img alt="HTML" loading="lazy" width="32" height="32" decoding="async" data-nimg="1"
                    class="img-tech drop-shadow-xl transition-all duration-300 h-[65%] w-[65%] lg:h-[85%] lg:w-[85%]  "
                    :src="item.imageUrl" style="color: transparent;">
                </div>
                <div class="flex items-center text-sm md:text-base lg:text-lg">
                  <div class="tech font-medium text-secondary transition-all duration-300 translate-y-0 ">{{ item.name }}
                  </div>
                  <div
                    class="status-tech opacity-0 absolute mt-5 text-[10px] text-amber-200 transition-all duration-300 md:text-xs lg:text-sm">
                    {{ item.status }}</div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div v-show="activeTab === 2">
          <div class="grid grid-cols-2 gap-4 pb-32 md:grid-cols-3 md:gap-8 xl:grid-cols-4 xl:gap-10 2xl:gap-12">
            <div v-for="item in tools" :key="item.id">
              <div
                class="item-tech flex cursor-pointer items-center gap-2 rounded border border-amber-200 px-2 py-2 hover:bg-amber-200 hover:bg-opacity-10 md:gap-3 lg:px-3">
                <div class="flex h-12 w-12 items-center justify-center p-0 lg:h-16 lg:w-16 lg:p-2 zoom-in">
                  <img alt="HTML" loading="lazy" width="32" height="32" decoding="async" data-nimg="1"
                    class="img-tech drop-shadow-xl transition-all duration-300 h-[65%] w-[65%] lg:h-[85%] lg:w-[85%]  "
                    :src="item.imageUrl" style="color: transparent;">
                </div>
                <div class="flex items-center text-sm md:text-base lg:text-lg">
                  <div class="tech font-medium text-secondary transition-all duration-300 translate-y-0 ">{{ item.name }}
                  </div>
                  <div
                    class="status-tech opacity-0 absolute mt-5 text-[10px] text-amber-200 transition-all duration-300 md:text-xs lg:text-sm">
                    {{ item.status }}</div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>
    </article>
  </div>
</template>

<style>
.fadein-left {
  opacity: 0;
  animation: fadeInLeft 0.5s ease-out forwards;
}

@keyframes fadeInLeft {
  0% {
    opacity: 0;
    transform: translateX(100%);
  }

  100% {
    opacity: 1;
    transform: translateX(0);
  }
}

.fadeins-1 {
  animation-delay: 500ms;
}

.fadeins-2 {
  animation-delay: 800ms;
}

.img-tech,
.tech {
  transition: transform 0.3s ease;
}

.item-tech:hover .img-tech {
  transform: scale(1.3);
}

.item-tech:hover .tech {
  transform: translateY(-12px);
}

.item-tech:hover .status-tech {
  opacity: 1;
}
</style>
