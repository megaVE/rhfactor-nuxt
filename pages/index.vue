<template>
  <main>
    <section
      class="hero-image w-full md:h-screen relative bg-cover overflow-y-hidden pb-8 md:pb-0"
    >
      <div class="absolute size-full top-0 left-0 bg-gradient-to-r from-[#1C3433E5]/90 to-[#1C3433E5]/40 z-20"></div>
      <Header class-name="bg-transparent" />
      <HomeBanner />
    </section>
    <section
      class="bg-[#2B2D3D] w-full md:h-screen flex flex-col-reverse md:flex-row"
    >
      <figure class="flex-1 md:overflow-hidden p-16 pt-0 md:p-0">
        <NuxtImg
          src="img/fred-home-in-company.jpg"
          alt="In Company"
          class="w-full rounded-3xl md:rounded-none"
        />
      </figure>
      <article class="flex-1">
        <div class="m-16">
          <div class="space-y-6 mb-8">
            <h2 class="section-title !text-[#53CC6C]">In Company</h2>
            <p class="article-text !text-white leading-[150%]">
              O maior desafio do RH é garantir um ambiente de trabalho produtivo
              e reter talentos. Fred Junco oferece treinamentos In Company
              personalizados que diagnosticam as necessidades da sua empresa e
              apresentam soluções práticas para aumentar a produtividade,
              reduzir turnover e melhorar a satisfação no ambiente corporativo.
            </p>
          </div>
          <InCompanyList />
          <div class="group relative flex w-full md:w-fit cursor-pointer">
            <span
              class="absolute inset-0 border border-transparent group-hover:border-[#53CC6C] group-hover:animate-ping rounded-md hidden md:inline"
            ></span>
            <NuxtLink
              to="/contact"
              class="mx-auto md:mx-0 link-button !inline-flex text-white border-none bg-[#53CC6C]"
            >
              Quero me cadastrar no In Company
            </NuxtLink>
          </div>
        </div>
      </article>
    </section>
    <section class="w-full md:h-screen flex flex-col md:flex-row">
      <article class="flex-1">
        <div class="m-16">
          <div class="space-y-6 mb-8">
            <h2 class="section-title !text-[#669997]">Mentoria Xeque-Mate</h2>
            <p class="article-text leading-[150%]">
              A Mentoria Xeque-Mate é um programa completo focado em vendas e
              experiência do cliente (CX). Desenvolvida por Fred Junco, a
              mentoria ajuda profissionais a aprimorar estratégias, técnicas e
              mindset para atingir resultados extraordinários no mercado.
            </p>
          </div>
          <CheckedList
            id="checkmate"
            :items="[
              'Para Empreendedores',
              'Para Líderes Comerciais',
              'Para Empresas que Faturam até 100k por Mês',
            ]"
          />
          <NuxtLink
            to="/contact"
            class="link-button mt-16 text-[#669997] border-[#669997] hover:bg-[#669997] hover:text-white !block md:!inline-block"
          >
            Quero conhecer a Mentoria
          </NuxtLink>
        </div>
      </article>
      <figure class="flex-1 md:overflow-hidden p-16 pt-0 md:p-0">
        <NuxtImg
          src="img/fred-home-checkmate.jpg"
          alt="In Company"
          class="w-full rounded-3xl md:rounded-none"
        />
      </figure>
    </section>
    <section class="w-full md:h-screen bg-[#FFF8F4] flex flex-col md:flex-row">
      <article class="flex-1">
        <div class="m-16">
          <div class="space-y-6 mb-8">
            <h2 class="section-title !text-[#E9763D]">Quick Wins</h2>
            <q
              class="flex md:block font-medium text-xl fh:text-3xl tracking-tight not-italic no-quotes"
            >
              <NuxtImg
                src="icons/quote-icon.svg"
                class="inline-block h-5 mr-2 self-start"
              />
              <span class="text-center md:text-left self-center">
                Aprendizados para colocar em ação e alcançar resultados
                imediatos
              </span>
              <NuxtImg
                src="icons/quote-icon.svg"
                class="inline-block rotate-180 h-5 ml-2 self-end"
              />
            </q>
            <p class="article-text leading-[150%]">
              Lorem, ipsum dolor sit amet consectetur adipisicing elit. Nam
              vitae doloremque a, vero cupiditate maxime aperiam fugiat deserunt
              accusantium mollitia eaque unde ad voluptatibus, iure iste
              perferendis temporibus odio molestias.
            </p>
          </div>
          <NuxtLink
            to="/contact"
            class="link-button mt-16 text-[#E9763D] border-[#E9763D] hover:bg-[#E9763D] hover:text-white !block md:!inline-block"
          >
            Quero adquirir meu livro
          </NuxtLink>
        </div>
      </article>
      <div class="flex-1 md:overflow-y-hidden p-16 pb-0">
        <figure
          class="relative bg-[#E9763D] rounded-3xl size-full overflow-hidden"
        >
          <NuxtImg
            src="img/fred-home-quick-wins.png"
            alt="Quick Wins"
            class="pt-20 fh:pt-40 md:pt-0 w-full md:scale-75 fh:scale-100 relative z-30"
          />
          <div
            class="size-full blur-[12rem] bg-[#FFA172] top-0 -translate-y-1/2 right-0 translate-x-1/2 absolute rounded-[50%] z-20"
          ></div>
          <div
            class="size-full blur-[12rem]bg-[#FFA578] bottom-0 translate-y-1/2 left-0 -translate-x-1/2 absolute rounded-[50%] z-20"
          ></div>
        </figure>
      </div>
    </section>
    <section class="space-y-16 py-16 md:py-24">
      <div class="mx-16 md:mx-48 flex flex-col md:flex-row items-center gap-8">
        <h2 class="section-title">Vídeos do Fred</h2>
        <p class="article-text leading-[150%] max-w-xl">
          Explore uma seleção de conteúdos exclusivos, incluindo palestras,
          vídeos e insights compartilhados por Fred Junco.
        </p>
        <PageController class-name="ml-auto hidden md:flex" />
      </div>
      <ul
        class="flex flex-col md:flex-row items-center text-white font-semibold text-xl fh:text-3xl text-center md:overflow-x-hidden gap-8 md:p-0 px-8"
      >
        <li
          class="group overflow-hidden md:h-[30rem] w-full md:w-96 md:first:ml-48 md:last:mr-48 rounded-2xl cursor-pointer"
        >
          <a
            href="#"
            class="relative group overflow-hidden flex flex-col justify-end items-center space-y-6 size-full p-8"
          >
            <figure class="absolute top-0 left-0 size-full">
              <div class="relative size-full">
                <NuxtImg
                  src="img/fred-video-1.jpg"
                  alt="Vídeo 1"
                  class="relative z-10 scale-175 group-hover:scale-200 duration-200"
                />
                <div
                  class="absolute top-0 left-0 size-full z-20 bg-gradient-to-t from-black/70 to-black/0"
                ></div>
              </div>
            </figure>
            <div class="md:space-y-6 z-30">
              <article class="space-y-1">
                <h4>Como me enganar como cliente em 7 passos</h4>
                <span class="text-base fh:text-xl font-normal">
                  05 abr de 2022
                </span>
              </article>
              <span
                href="#"
                class="text-lg fh:text-3x hover:underline hidden md:inline"
              >
                Acessar agora
                <NuxtImg
                  src="icons/arrow-up-right-icon.svg"
                  alt="->"
                  class="ml-2 size-4 inline-block white-filter"
                />
              </span>
            </div>
          </a>
        </li>
        <li
          class="group overflow-hidden md:h-[30rem] w-full md:w-96 md:first:ml-48 md:last:mr-48 rounded-2xl cursor-pointer"
        >
          <a
            href="#"
            class="relative group overflow-hidden flex flex-col justify-end items-center space-y-6 size-full p-8"
          >
            <figure class="absolute top-0 left-0 size-full">
              <div class="relative size-full">
                <NuxtImg
                  src="img/fred-video-2.jpg"
                  alt="Vídeo 2"
                  class="relative z-10 scale-175 group-hover:scale-200 duration-200"
                />
                <div
                  class="absolute top-0 left-0 size-full z-20 bg-gradient-to-t from-black/70 to-black/0"
                ></div>
              </div>
            </figure>
            <div class="md:space-y-6 z-30">
              <article class="space-y-1">
                <h4>Como me enganar como cliente em 7 passos</h4>
                <span class="text-base fh:text-xl font-normal">
                  05 abr de 2022
                </span>
              </article>
              <span
                href="#"
                class="text-lg fh:text-3x hover:underline hidden md:inline"
              >
                Acessar agora
                <NuxtImg
                  src="icons/arrow-up-right-icon.svg"
                  alt="->"
                  class="ml-2 size-4 inline-block white-filter"
                />
              </span>
            </div>
          </a>
        </li>
        <li
          class="group overflow-hidden md:h-[30rem] w-full md:w-96 md:first:ml-48 md:last:mr-48 rounded-2xl cursor-pointer"
        >
          <a
            href="#"
            class="relative group overflow-hidden flex flex-col justify-end items-center space-y-6 size-full p-8"
          >
            <figure class="absolute top-0 left-0 size-full">
              <div class="relative size-full">
                <NuxtImg
                  src="img/fred-video-3.jpg"
                  alt="Vídeo 3"
                  class="relative z-10 scale-175 group-hover:scale-200 duration-200"
                />
                <div
                  class="absolute top-0 left-0 size-full z-20 bg-gradient-to-t from-black/70 to-black/0"
                ></div>
              </div>
            </figure>
            <div class="md:space-y-6 z-30">
              <article class="space-y-1">
                <h4>Como me enganar como cliente em 7 passos</h4>
                <span class="text-base fh:text-xl font-normal">
                  05 abr de 2022
                </span>
              </article>
              <span
                href="#"
                class="text-lg fh:text-3x hover:underline hidden md:inline"
              >
                Acessar agora
                <NuxtImg
                  src="icons/arrow-up-right-icon.svg"
                  alt="->"
                  class="ml-2 size-4 inline-block white-filter"
                />
              </span>
            </div>
          </a>
        </li>
        <li
          class="group overflow-hidden md:h-[30rem] w-full md:w-96 md:first:ml-48 md:last:mr-48 rounded-2xl cursor-pointer"
        >
          <a
            href="#"
            class="relative group overflow-hidden flex flex-col justify-end items-center space-y-6 size-full p-8"
          >
            <figure class="absolute top-0 left-0 size-full">
              <div class="relative size-full">
                <NuxtImg
                  src="img/fred-video-4.jpg"
                  alt="Vídeo 4"
                  class="relative z-10 scale-175 group-hover:scale-200 duration-200"
                />
                <div
                  class="absolute top-0 left-0 size-full z-20 bg-gradient-to-t from-black/70 to-black/0"
                ></div>
              </div>
            </figure>
            <div class="md:space-y-6 z-30">
              <article class="space-y-1">
                <h4>Como me enganar como cliente em 7 passos</h4>
                <span class="text-base fh:text-xl font-normal">
                  05 abr de 2022
                </span>
              </article>
              <span
                href="#"
                class="text-lg fh:text-3x hover:underline hidden md:inline"
              >
                Acessar agora
                <NuxtImg
                  src="icons/arrow-up-right-icon.svg"
                  alt="->"
                  class="ml-2 size-4 inline-block white-filter"
                />
              </span>
            </div>
          </a>
        </li>
        <li
          class="group overflow-hidden md:h-[30rem] w-full md:w-96 md:first:ml-48 md:last:mr-48 rounded-2xl cursor-pointer"
        >
          <a
            href="#"
            class="relative group overflow-hidden flex flex-col justify-end items-center space-y-6 size-full p-8"
          >
            <figure class="absolute top-0 left-0 size-full">
              <div class="relative size-full">
                <NuxtImg
                  src="img/fred-video-5.jpg"
                  alt="Vídeo 5"
                  class="relative z-10 scale-175 group-hover:scale-200 duration-200"
                />
                <div
                  class="absolute top-0 left-0 size-full z-20 bg-gradient-to-t from-black/70 to-black/0"
                ></div>
              </div>
            </figure>
            <div class="md:space-y-6 z-30">
              <article class="space-y-1">
                <h4>Como me enganar como cliente em 7 passos</h4>
                <span class="text-base fh:text-xl font-normal">
                  05 abr de 2022
                </span>
              </article>
              <span
                href="#"
                class="text-lg fh:text-3x hover:underline hidden md:inline"
              >
                Acessar agora
                <NuxtImg
                  src="icons/arrow-up-right-icon.svg"
                  alt="->"
                  class="ml-2 size-4 inline-block white-filter"
                />
              </span>
            </div>
          </a>
        </li>
      </ul>
      <div class="flex justify-center mx-8 md:mx-0">
        <a to="#" class="group link-button green"
          >Acesse o canal do Fred Junco
          <NuxtImg
            src="icons/arrow-up-right-icon.svg"
            alt="->"
            class="md:ml-4 size-5 inline-block group-hover:white-filter"
          />
        </a>
      </div>
    </section>
    <section class="bg-[#F5F2EC] py-16 md:p-24 space-y-16">
      <div class="mx-16 md:mx-48 flex flex-col md:flex-row items-center gap-8">
        <h2 class="section-title">Blog do Fred</h2>
        <p class="article-text leading-[150%] max-w-xl">
          Explore conteúdos e artigos sobre o mundo do RH e relações
          interpessoais compartilhados por Fred Junco.
        </p>
      </div>
      <ul
        class="flex flex-col md:flex-row items-center font-semibold text-[#1C3433] text-xl fh:text-3xl gap-8 px-16"
      >
        <li class="group flex flex-col md:w-1/3 cursor-pointer">
          <figure class="relative overflow-hidden h-80 w-full rounded-t-3xl">
            <NuxtImg
              src="img/fred-blog-1.jpg"
              alt="Post 1"
              class="size-full absolute top-0 left-0 object-cover object-center group-hover:scale-125 duration-200"
            />
          </figure>
          <div
            class="p-8 md:space-y-6 bg-white rounded-b-3xl text-center md:text-left"
          >
            <h4>Como me enganar como cliente em 7 passos</h4>
            <span
              href="#"
              class="text-lg fh:text-2xl text-[#53CC6C] hover:underline hidden md:inline"
            >
              Ver conteúdo
              <NuxtImg
                src="icons/arrow-up-right-icon.svg"
                alt="->"
                class="size-4 inline-block"
              />
            </span>
          </div>
        </li>
        <li class="group flex flex-col md:w-1/3 cursor-pointer">
          <figure class="relative overflow-hidden h-80 w-full rounded-t-3xl">
            <NuxtImg
              src="img/fred-blog-2.jpg"
              alt="Post 2"
              class="size-full absolute top-0 left-0 object-cover object-center group-hover:scale-125 duration-200"
            />
          </figure>
          <div
            class="p-8 md:space-y-6 bg-white rounded-b-3xl text-center md:text-left"
          >
            <h4>Como me enganar como cliente em 7 passos</h4>
            <span
              href="#"
              class="text-lg fh:text-2xl text-[#53CC6C] hover:underline hidden md:inline"
            >
              Ver conteúdo
              <NuxtImg
                src="icons/arrow-up-right-icon.svg"
                alt="->"
                class="size-4 inline-block"
              />
            </span>
          </div>
        </li>
        <li
          class="group flex flex-col md:w-1/3 cursor-pointer text-center md:text-left"
        >
          <figure class="relative overflow-hidden h-80 w-full rounded-t-3xl">
            <NuxtImg
              src="img/fred-blog-3.jpg"
              alt="Post 3"
              class="size-full absolute top-0 left-0 object-cover object-center group-hover:scale-125 duration-200"
            />
          </figure>
          <div class="p-8 md:space-y-6 bg-white rounded-b-3xl">
            <h4>Como me enganar como cliente em 7 passos</h4>
            <span
              href="#"
              class="text-lg fh:text-2xl text-[#53CC6C] hover:underline hidden md:inline"
            >
              Ver conteúdo
              <NuxtImg
                src="icons/arrow-up-right-icon.svg"
                alt="->"
                class="size-4 inline-block"
              />
            </span>
          </div>
        </li>
      </ul>
      <div class="flex justify-center">
        <a to="#" class="group link-button green"
          >Acesse o blog do Fred Junco
          <NuxtImg
            src="icons/arrow-up-right-icon.svg"
            alt="->"
            class="ml-4 size-5 inline-block group-hover:white-filter"
          />
        </a>
      </div>
    </section>
    <section class="p-16 flex flex-col md:flex-row items-center">
      <div class="flex-1 md:p-16">
        <NuxtImg
          src="img/fred-home-contact.jpg"
          alt="Fred Junco"
          class="rounded-3xl"
        />
      </div>
      <div class="flex-1 py-8 md:p-16 space-y-8">
        <h2 class="section-title">Quem é Fred Junco?</h2>
        <h3 class="font-bold text-base fh:text-xl text-[#1C3433] uppercase">
          PALESTRANTE | LIDERANÇA | NEGOCIAÇÃO | NEUROVENDAS | TREINAMENTO
          CORPORATIVO | GESTÃO COMERCIAL
        </h3>
        <p class="article-text">
          Com uma formação robusta e mais de 20 anos de experiência em liderança
          e vendas, Fred Junco é reconhecido por sua abordagem estratégica e
          personalizada. Sua metodologia exclusiva de treinamento já ajudou
          milhares de profissionais a atingirem resultados extraordinários.
          Conheça suas conquistas, prêmios e metodologias que fazem a diferença
          no mercado corporativo.
        </p>
        <a to="#" class="group link-button green !block md:!inline-block">
          Quero falar com o Fred Junco

          <NuxtImg
            src="icons/arrow-up-right-icon.svg"
            alt="->"
            class="ml-4 size-5 inline-block group-hover:white-filter"
          />
        </a>
      </div>
    </section>
    <ClientSection />
    <HomeSpotlight />
  </main>
  <Footer />
</template>

<script setup>
import HomeBanner from "~/components/HomeBanner.vue";
import HomeSpotlight from "~/components/HomeSpotlight.vue";

useHead({
  title: "Fred Junco - Conexões e Negócios",
});
</script>
