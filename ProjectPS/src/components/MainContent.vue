<template>
  <div class="md:ml-[25%] bg-white min-h-screen relative text-gray-700">
    <nav
      class="sticky top-0 z-50 bg-white/90 backdrop-blur-md border-b border-gray-200 px-8 py-6 shadow-sm"
    >
      <ul
        class="flex justify-center md:justify-end gap-12 font-bold text-gray-500 text-lg uppercase tracking-wider"
      >
        <li>
          <button @click="moveTo('intro-section')" class="hover:text-emerald-600 transition">
            Home
          </button>
        </li>
        <li>
          <button @click="moveTo('resume-section')" class="hover:text-emerald-600 transition">
            Resume
          </button>
        </li>
        <li>
          <button @click="moveTo('project-section')" class="hover:text-emerald-600 transition">
            Projects
          </button>
        </li>
        <li>
          <button @click="moveTo('skill-section')" class="hover:text-emerald-600 transition">
            Skills
          </button>
        </li>
      </ul>
    </nav>

    <section
      id="intro-section"
      class="min-h-[90vh] flex flex-col justify-center items-center p-10 bg-gray-50"
    >
      <h1 class="text-5xl font-bold mb-16 text-gray-900">백엔드 개발자 포트폴리오</h1>
      <p class="text-center text-xl text-gray-500 mb-20">
        안녕하세요. <br />
        꾸준히 성장하는 개발자 <br />
        김민우입니다.
      </p>

      <div class="flex gap-6">
        <button
          @click="moveTo('project-section')"
          class="px-12 py-4 bg-gray-800 text-white rounded-full font-bold text-lg hover:bg-emerald-600 transition shadow-lg transform hover:-translate-y-1"
        >
          Project
        </button>

        <button
          @click="moveTo('skill-section')"
          class="px-8 py-4 bg-white border-2 border-gray-800 text-gray-800 rounded-full font-bold text-lg hover:border-emerald-500 hover:text-emerald-500 transition shadow-lg transform hover:-translate-y-1"
        >
          Main Skills
        </button>
      </div>
    </section>

    <section id="resume-section" class="py-24 px-8 md:px-20 border-t border-gray-100">
      <div
        class="flex flex-col md:flex-row md:items-end justify-between mb-16 border-b-4 border-emerald-100 pb-2"
      >
        <h2 class="text-3xl font-bold text-emerald-600">Resume</h2>

        <div class="flex flex-col sm:flex-row gap-3 mt-6 md:mt-0">
          <a
            href="/이력서.pdf"
            target="_blank"
            class="w-44 flex items-center justify-center gap-2 px-5 py-2 bg-white border-2 border-gray-800 text-gray-800 rounded-lg hover:border-emerald-500 hover:text-emerald-500 hover:-translate-y-1 transition shadow-md font-bold text-sm"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke-width="2"
              stroke="currentColor"
              class="w-5 h-5"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                d="M19.5 14.25v-2.625a3.375 3.375 0 00-3.375-3.375h-1.5A1.125 1.125 0 0113.5 7.125v-1.5a3.375 3.375 0 00-3.375-3.375H8.25m0 12.75h7.5m-7.5 3H12M10.5 2.25H5.625c-.621 0-1.125.504-1.125 1.125v17.25c0 .621.504 1.125 1.125 1.125h12.75c.621 0 1.125-.504 1.125-1.125V11.25a9 9 0 00-9-9z"
              />
            </svg>
            이력서 보기
          </a>

          <a
            href="/자기소개서.pdf"
            target="_blank"
            class="w-44 flex items-center justify-center gap-2 px-5 py-2 bg-gray-800 text-white rounded-lg hover:bg-emerald-600 hover:-translate-y-1 transition shadow-md font-bold text-sm"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke-width="2"
              stroke="currentColor"
              class="w-5 h-5"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                d="M19.5 14.25v-2.625a3.375 3.375 0 00-3.375-3.375h-1.5A1.125 1.125 0 0113.5 7.125v-1.5a3.375 3.375 0 00-3.375-3.375H8.25m0 12.75h7.5m-7.5 3H12M10.5 2.25H5.625c-.621 0-1.125.504-1.125 1.125v17.25c0 .621.504 1.125 1.125 1.125h12.75c.621 0 1.125-.504 1.125-1.125V11.25a9 9 0 00-9-9z"
              />
            </svg>
            자기소개서 보기
          </a>
        </div>
      </div>

      <div class="mb-16">
        <h3 class="text-xl font-bold text-gray-900 mb-8 flex items-center">
          <span class="w-2 h-8 bg-gray-800 mr-3 rounded-sm"></span>About Me
        </h3>

        <div class="grid grid-cols-1 md:grid-cols-2 gap-y-10 gap-x-12">
          <div>
            <span class="block text-gray-400 text-xs font-bold tracking-widest mb-1">NAME</span>
            <p class="text-xl text-gray-900 font-bold mb-6">김민우</p>

            <span class="block text-gray-400 text-xs font-bold tracking-widest mb-1"
              >BIRTH DATE</span
            >
            <p class="text-lg text-gray-700 mb-6">1999.02.21</p>
            <span class="block text-gray-400 text-xs font-bold tracking-widest mb-1">LOCATION</span>
            <p class="text-lg text-gray-700 mb-6">인천광역시 계양구</p>
            <span class="block text-gray-400 text-xs font-bold tracking-widest mb-1">CONTACT</span>
            <p class="text-lg text-gray-700">kimminu0221@gmail.com</p>
          </div>

          <div>
            <span
              class="block text-emerald-600 text-xs font-bold tracking-widest mb-4 border-b border-gray-200 pb-2"
              >EDUCATION</span
            >
            <ul class="space-y-6">
              <li>
                <div class="flex justify-between items-baseline">
                  <strong class="text-lg text-gray-800">인하공업전문대학교</strong>
                  <span class="text-sm text-gray-500">2023.03 ~ 2026.02</span>
                </div>
                <p class="text-gray-600">컴퓨터정보공학과 (졸업예정) | 4.1 / 4.5</p>
              </li>
              <li>
                <div class="flex justify-between items-baseline">
                  <strong class="text-lg text-gray-800">한서대학교</strong>
                  <span class="text-sm text-gray-500">2017.03 ~ 2022.08</span>
                </div>
                <p class="text-gray-600">항공전자공학 (2학년 수료)</p>
                <p class="text-xs text-gray-400 mt-1">- 소프트웨어 개발로 진로 변경</p>
              </li>
              <li>
                <div class="flex justify-between items-baseline">
                  <strong class="text-lg text-gray-800">계산공업고등학교</strong>
                  <span class="text-sm text-gray-500">2014.03 ~ 2017.02</span>
                </div>
                <p class="text-gray-600">컴퓨터정보전자과 (졸업)</p>
              </li>
            </ul>
          </div>
        </div>
      </div>

      <div>
        <h3 class="text-xl font-bold text-gray-900 mb-6 flex items-center">
          <span class="w-2 h-8 bg-gray-800 mr-3 rounded-sm"></span>Certificates & Awards
        </h3>
        <ul class="grid grid-cols-1 md:grid-cols-2 gap-4">
          <li class="bg-gray-50 p-4 rounded border border-gray-200 border-l-4 border-l-emerald-500">
            <div>
              <strong class="block text-gray-900 mb-1">
                2025 동계 한국컴퓨터정보학회 우수논문상</strong
              >
              <span class="text-sm text-gray-500">한국컴퓨터정보학회 | 2025.01</span>
              <p class="text-xs text-gray-500 mt-2">
                주제: 통합 일기예보와 함께 지속적인 계획 관리를 위한 모바일 애플리케이션 개발
              </p>
            </div>
            <a
              href="https://www.dbpia.co.kr/journal/articleDetail?nodeId=NODE12098896"
              target="_blank"
              class="text-sm font-bold text-emerald-600 hover:text-emerald-800 hover:underline flex items-center gap-1 w-fit"
            >
              🔗 논문/자료 링크
            </a>
          </li>
          <li class="bg-gray-50 p-4 rounded border border-gray-200">
            <strong class="block text-gray-900 mb-1">SQLD</strong>
            <span class="text-sm text-gray-500">한국데이터산업진흥원 | 2024.09</span>
          </li>
          <li class="bg-gray-50 p-4 rounded border border-gray-200">
            <strong class="block text-gray-900 mb-1">MOS Master</strong>
            <span class="text-sm text-gray-500">YBMIT | 2023.12</span>
          </li>
          <li class="bg-gray-50 p-4 rounded border border-gray-200">
            <strong class="block text-gray-900 mb-1">1종 보통 운전면허</strong>
            <span class="text-sm text-gray-500">서울지방경찰청 | 2020.08</span>
          </li>
          <li class="bg-gray-50 p-4 rounded border border-gray-200">
            <strong class="block text-gray-900 mb-1">전자기능사</strong>
            <span class="text-sm text-gray-500">한국산업인력공단 | 2016.07</span>
          </li>
        </ul>
      </div>
    </section>

    <section id="project-section" class="py-24 px-8 md:px-20 bg-gray-50 border-t border-gray-200">
      <h2
        class="text-3xl font-bold mb-16 text-emerald-600 inline-block border-b-4 border-emerald-200 pb-2"
      >
        Projects
      </h2>

      <div class="space-y-12">
        <article
          class="bg-white p-8 rounded-xl shadow-sm hover:shadow-md transition cursor-pointer group"
          onclick="window.open('https://github.com/mainu0221/ProjectAndroid')"
        >
          <div class="flex flex-col md:flex-row gap-8">
            <div
              class="w-full md:w-1/3 h-48 bg-gray-100 rounded-lg overflow-hidden relative border border-gray-200"
            >
              <img
                src="/images/Triplan.jpg"
                alt="프로젝트 미리보기"
                class="w-full h-full object-cover object-top group-hover:scale-105 transition duration-500"
                loading="lazy"
              />
            </div>
            <div class="w-full md:w-2/3">
              <h3 class="text-2xl font-bold mb-3 group-hover:text-emerald-600 transition">
                Triplan
              </h3>
              <p class="text-gray-600 mb-4 leading-relaxed">
                AndroidStudio와 RoomDatabase를 이용하여 날씨, 캘린더, 체크리스트 <br />
                세가지 기능을 합친 어플리케이션입니다.
              </p>
              <div class="flex gap-2 flex-wrap">
                <span
                  class="px-3 py-1 bg-emerald-50 text-emerald-700 text-sm font-medium rounded-full"
                  >우수논문상</span
                >
                <span
                  class="px-3 py-1 bg-emerald-50 text-emerald-700 text-sm font-medium rounded-full"
                  >AndroidStudio</span
                >
                <span
                  class="px-3 py-1 bg-emerald-50 text-emerald-700 text-sm font-medium rounded-full"
                  >Java</span
                >
                <span
                  class="px-3 py-1 bg-emerald-50 text-emerald-700 text-sm font-medium rounded-full"
                  >RoomDatabase</span
                >
              </div>
            </div>
          </div>
        </article>

        <article
          class="bg-white p-8 rounded-xl shadow-sm hover:shadow-md transition cursor-pointer group"
          onclick="window.open('https://www.notion.so/RT-2b394fc9c7c780dcba92df657ff1770c')"
        >
          <div class="flex flex-col md:flex-row gap-8">
            <div
              class="w-full md:w-1/3 h-48 bg-gray-100 rounded-lg overflow-hidden relative border border-gray-200"
            >
              <img
                src="/images/Fermata.png"
                alt="프로젝트 미리보기"
                class="w-full h-full object-cover object-top group-hover:scale-105 transition duration-500"
                loading="lazy"
              />
            </div>
            <div class="w-full md:w-2/3">
              <h3 class="text-2xl font-bold mb-3 group-hover:text-emerald-600 transition">
                2D 횡스크롤 로그라이트 게임 : 페르마타
              </h3>
              <p class="text-gray-600 mb-4 leading-relaxed">
                도트그래픽과 Unity엔진을 이용한 횡스크롤 2D 로그라이트 게임 입니다.
              </p>
              <div class="flex gap-2 flex-wrap">
                <span
                  class="px-3 py-1 bg-emerald-50 text-emerald-700 text-sm font-medium rounded-full"
                  >Unity</span
                >
                <span
                  class="px-3 py-1 bg-emerald-50 text-emerald-700 text-sm font-medium rounded-full"
                  >Unity DevOps Version Control</span
                >
                <span
                  class="px-3 py-1 bg-emerald-50 text-emerald-700 text-sm font-medium rounded-full"
                  >C#</span
                >
                <span
                  class="px-3 py-1 bg-emerald-50 text-emerald-700 text-sm font-medium rounded-full"
                  >Sprite</span
                >
              </div>
            </div>
          </div>
        </article>

        <article
          class="bg-white p-8 rounded-xl shadow-sm hover:shadow-md transition cursor-pointer group"
          onclick="window.open('https://github.com/mainu0221/JspProject')"
        >
          <div class="flex flex-col md:flex-row gap-8">
            <div
              class="w-full md:w-1/3 h-48 bg-gray-100 rounded-lg overflow-hidden relative border border-gray-200"
            >
              <img
                src="/images/FortuneTelling.png"
                alt="프로젝트 미리보기"
                class="w-full h-full object-cover object-top group-hover:scale-105 transition duration-500"
                loading="lazy"
              />
            </div>
            <div class="w-full md:w-2/3">
              <h3 class="text-2xl font-bold mb-3 group-hover:text-emerald-600 transition">
                운세보기 사이트
              </h3>
              <p class="text-gray-600 mb-4 leading-relaxed">
                OpenAI API ChatGPT 3.5를 이용한 오늘의 운세보기 사이트 입니다.
              </p>
              <div class="flex gap-2 flex-wrap">
                <span
                  class="px-3 py-1 bg-emerald-50 text-emerald-700 text-sm font-medium rounded-full"
                  >Jsp</span
                >
                <span
                  class="px-3 py-1 bg-emerald-50 text-emerald-700 text-sm font-medium rounded-full"
                  >Java</span
                >
                <span
                  class="px-3 py-1 bg-emerald-50 text-emerald-700 text-sm font-medium rounded-full"
                  >MySQL</span
                >
                <span
                  class="px-3 py-1 bg-emerald-50 text-emerald-700 text-sm font-medium rounded-full"
                  >OpoenAI API</span
                >
              </div>
            </div>
          </div>
        </article>
      </div>
    </section>

    <section id="skill-section" class="py-24 px-8 md:px-20 border-t border-gray-200 bg-gray-50">
      <h2
        class="text-3xl font-bold mb-16 text-emerald-600 inline-block border-b-4 border-emerald-100 pb-2"
      >
        Main Skills
      </h2>

      <div class="flex flex-wrap justify-center gap-6 text-center">
        <div
          class="w-40 p-6 bg-white border border-gray-200 rounded-xl cursor-default group shadow-sm flex flex-col items-center"
        >
          <img
            src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg"
            alt="Python"
            class="w-16 h-16 mb-4 object-contain"
          />
          <div class="font-bold text-lg text-gray-700">Python</div>
        </div>

        <div
          class="w-40 p-6 bg-white border border-gray-200 rounded-xl cursor-default group shadow-sm flex flex-col items-center"
        >
          <img
            src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/csharp/csharp-original.svg"
            alt="C#"
            class="w-16 h-16 mb-4 object-contain"
          />
          <div class="font-bold text-lg text-gray-700">C#</div>
        </div>

        <div
          class="w-40 p-6 bg-white border border-gray-200 rounded-xl cursor-default group shadow-sm flex flex-col items-center"
        >
          <img
            src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original.svg"
            alt="Java"
            class="w-16 h-16 mb-4 object-contain"
          />
          <div class="font-bold text-lg text-gray-700">Java</div>
        </div>

        <div
          class="w-40 p-6 bg-white border border-gray-200 rounded-xl cursor-default group shadow-sm flex flex-col items-center"
        >
          <img
            src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg"
            alt="Git"
            class="w-16 h-16 mb-4 object-contain"
          />
          <div class="font-bold text-lg text-gray-700">Git/GitHub</div>
        </div>

        <div
          class="w-40 p-6 bg-white border border-gray-200 rounded-xl cursor-default group shadow-sm flex flex-col items-center"
        >
          <img
            src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/notion/notion-original.svg"
            alt="Notion"
            class="w-16 h-16 mb-4 object-contain"
          />
          <div class="font-bold text-lg text-gray-700">Notion</div>
        </div>
      </div>
    </section>

    <div class="h-40"></div>
  </div>
</template>

<script setup>
const moveTo = (id) => {
  const el = document.getElementById(id)
  if (el) {
    const headerOffset = 70 // 메뉴바 높이 + 여백
    const elementPosition = el.getBoundingClientRect().top
    const offsetPosition = elementPosition + window.pageYOffset - headerOffset

    window.scrollTo({
      top: offsetPosition,
      behavior: 'smooth',
    })
  }
}
</script>
