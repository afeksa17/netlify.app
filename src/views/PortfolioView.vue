<script>
export default {
  data() {
    return {
      activeTab: 1,
      items: [
        {
          id: 1,
          name: 'Github',
          imageUrl: 'portfolio_v2',
          status: 'My personal website, I created this website to display my profile, skills and projects. As well as my place to try new technology.',
          tech: 'VueJS 3, Tailwind',
          github: 'https://github.com/afeksa17',
          demo: 'null'
        },
        {
          id: 13,
          name: 'Motion Graphic',
          imageUrl: 'motiongraphic',
          status: 'Create visual effects and motion graphics for a video highlight for an esports film',
          tech: 'Adobe After Effect, Adobe Premiere, ',
          github: 'null',
          demo: 'https://drive.google.com/drive/folders/1nKKqN3jqz6z45CCgVDs2vbQ5IJtId2qe?usp=sharing'
        },
        {
          id: 2,
          name: 'DailyAct',
          imageUrl: 'DailyAct',
          status: 'Worked as a designer and front end developer at a company PT Amber Media Social, To create interesting social media applications.',
          tech: 'JavaScript, Adobe XD, Photoshop',
          github: 'null',
          demo: 'https://twitter.com/DailyactID'
        },
        {
          id: 3,
          name: 'Seruni',
          imageUrl: 'seruni',
          status: 'Company operating in the food ingredients sector, I am a web developer and content creator for this company.',
          tech: 'JavaScript, Photoshop',
          github: 'null',
          demo: 'https://www.linkedin.com/company/pt-sumber-rasa-nusantara-industri/about/'
        },
        {
          id: 4,
          name: 'JakCloth',
          imageUrl: 'folder',
          status: 'Making designs for clothes at the Jakcloth company, a company that sells clothing.',
          tech: 'Photoshop, Illustrator',
          github: 'null',
          demo: 'https://jakcloth.id/'
        },
        {
          id: 5,
          name: 'Nutrilicious',
          imageUrl: 'nutri',
          status: 'Shooting and editing videos for Nutrilicious Instagram and creating designs for Instagram.',
          tech: 'Premiere Pro, After Effect, Photoshop',
          github: 'null',
          demo: 'https://www.instagram.com/nutrilicious.katering/'
        },
        {
          id: 6,
          name: 'Hadi Kitchen',
          imageUrl: 'hadi',
          status: 'Shooting and editing videos, Nutrillicious is in the Hadi group too',
          tech: 'Premiere Pro, After Effect',
          github: 'null',
          demo: 'https://www.instagram.com/hadikitchen_id/'
        },
        {
          id: 7,
          name: 'Honest Beauty',
          imageUrl: 'Honest',
          status: 'Doing photos for Honest Beauty products,',
          tech: 'Sony A7 Mark III',
          github: 'null',
          demo: 'https://www.honest.com/beauty-products/view-all-beauty'
        },
        {
          id: 8,
          name: 'Imoki',
          imageUrl: 'Imoki',
          status: 'Take product photos and several designs to upload on Instagram',
          tech: 'Cannon 1D',
          github: 'null',
          demo: 'https://www.instagram.com/imokicoffee/'
        },
        {
          id: 9,
          name: 'Alter Ego X Detikcom',
          imageUrl: 'Esport',
          status: 'Rough cut editing and online editing for 21 episode films.',
          tech: 'Premiere Pro, After Effect, Davinci Resolve',
          github: 'null',
          demo: 'https://www.instagram.com/nutrilicious.katering/'
        },
        {
          id: 10,
          name: 'Instagram',
          imageUrl: 'instagram2',
          status: 'I have uploaded several posts on social media, but I dont upload them too regularly on Instagram',
          tech: 'Social Media',
          github: 'null',
          demo: 'https://www.instagram.com/afeksa_/'
        },
        {
          id: 11,
          name: 'Tiktok',
          imageUrl: 'tiktok',
          status: 'I just uploaded an editing video about the Valorant game on TikTok.',
          tech: 'Social Media',
          github: 'null',
          demo: 'https://www.tiktok.com/@afeksa17',
        },
        {
          id: 12,
          name: 'Linkedin',
          imageUrl: 'linkedin',
          status: 'Everything about me is on social media linkedin.',
          tech: 'Social Media',
          github: 'null',
          demo: 'https://www.linkedin.com/in/afif-eka-saputra/'
        },
      ]
    };
  }
}
</script>
<template>
  <div class="px-5 py-5 md:px-12 md:py-10 text-left text-amber-50 mx-3">
    <article data-page="about">
      <header>
        <div
          class="text-2xl font-bold text-white mb-10 fadein-bot title-section flex items-center justify-center flex-col">
          <!-- <div class="h-[1px] w-10 bg-amber-200 md:w-20 aos-init aos-animate"></div> -->
          <h4>Past Project Experience</h4>
          <h4 class="text-base font-normal text-transparent bg-clip-text bg-gradient-to-r from-slate-100 to-amber-300">
            Explore the projects I've worked on so far</h4>
        </div>
      </header>
      <section>
        <div>
          <div class="grid grid-cols-1 gap-4 pb-32 md:grid-cols-3 md:gap-3 xl:grid-cols-3 xl:gap-3 2xl:gap-5 fade-zoom-in">
            <div v-for="item in items" :key="item.id">
              <div
                class="item-card flex flex-col items-center gap-2 rounded bg-[#1e1e1f] hover:bg-[#282828] border border-[#383838] rounded-xl text-amber-50 md:gap-3 px-5 py-5 lg:px-5 ">
                <div class="flex h-12 w-12 items-center justify-center p-0 h-full w-full lg:p-0 zoom-in">
                  <img alt="HTML" loading="lazy" decoding="async" data-nimg="1" class="drop-shadow-xl rounded rounded-xl"
                    :src="'/img/portfolio-' + item.imageUrl + '.png'">
                </div>
                <div class="w-full flex flex-col gap-2 items-center text-sm md:text-base lg:text-lg">
                  <div class="title-text font-medium text-secondary">{{ item.name }}
                  </div>
                  <div class="w-full text-left text-[10px] text-[#c1c1c1] md:text-xs lg:text-sm">
                    {{ item.status }}</div>
                  <div class="w-full mt-4 text-normal text-sm text-left text-amber-200">
                    {{ item.tech }}
                  </div>
                  <div class="w-full flex justify-end">
                    <div class="flex cursor-pointer items-end gap-2 text-primary">
                      <a v-if="item.github !== 'null'"
                        :href="item.github" target="_blank" rel="noreferrer"
                        title="View github repository" class="transition-all hover:text-accent">
                        <svg stroke="currentColor"
                          fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round"
                          height="16" width="16" xmlns="http://www.w3.org/2000/svg">
                          <path
                            d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22">
                          </path>
                        </svg></a>
                        <a v-if="item.demo !== 'null'" :href="item.demo" target="_blank" rel="noreferrer"
                        title="View finished project" class="transition-all hover:text-accent">
                        <svg stroke="currentColor"
                          fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round"
                          height="18" width="18" xmlns="http://www.w3.org/2000/svg">
                          <path d="M18 13v6a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h6"></path>
                          <polyline points="15 3 21 3 21 9"></polyline>
                        <line x1="10" y1="14" x2="21" y2="3"></line>
                      </svg></a></div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </article>
</div></template>

<style>
.item-card:hover {
  transition: transform 0.3s ease;
  transform: translateY(-8px);
}
svg:hover{
  stroke: #ffdb70;
}
@keyframes fadeZoomIn {
  0% {
    opacity: 0;
    transform: scale(0.5);
  }
  100% {
    opacity: 1;
    transform: scale(1);
  }
}

/* Menggunakan animasi pada elemen yang diinginkan */
.fade-zoom-in {
  animation: fadeZoomIn 1s ease-in-out;
}
</style>