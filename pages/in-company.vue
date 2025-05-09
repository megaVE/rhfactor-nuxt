<template>
  <Header />
  <main>
    <section class="p-16 space-y-16">
      <h2 class="font-bold text-5xl text-[#1C3433]">In Company</h2>
      <div class="flex flex-col md:flex-row">
        <div class="flex-1 space-y-16">
          <NuxtImg
            src="img/fred-in-company.jpg"
            alt="Fred Junco In Company"
            class="max-h-screen rounded-3xl"
          />
        </div>
        <article class="flex-1 px-16">
          <div class="space-y-8 mb-8">
            <p class="font-normal text-lg text-[#6B6A66]">
              O maior desafio do RH é garantir um ambiente de trabalho
              produtivo, reter talentos e reduzir custos com turnover. Cada
              colaborador perdido representa um investimento desperdiçado em
              treinamento e desenvolvimento. Com o método exclusivo de Fred
              Junco, realizamos um diagnóstico preciso para identificar os
              pontos de melhoria nos processos internos da sua empresa. A partir
              disso, estruturamos treinamentos personalizados, focados em
              soluções reais para o seu time.
            </p>
            <p class="font-normal text-lg text-[#6B6A66]">
              Nosso objetivo é otimizar o desempenho, aumentar o faturamento e
              elevar a qualidade no ambiente corporativo. Com uma abordagem
              estratégica e prática, ajudamos sua equipe a trabalhar com mais
              engajamento, produtividade e satisfação.
            </p>
            <InCompanyList class-name="text-[#1C3433]" />
          </div>
        </article>
      </div>
    </section>
    <section class="space-y-16 py-16 overflow-x-hidden">
      <h2 class="font-bold text-5xl text-[#1C3433] text-center">
        Como Funciona
      </h2>
      <ul class="text-[#6B6A66] text-lg font-normal text-center flex">
        <li class="w-xl relative space-y-8 p-4">
          <NuxtImg
            class="h-14 absolute top-0 right-0 translate-x-1/2"
            src="icons/next-step-icon.svg"
            alt="->"
          />
          <div
            class="bg-[#C4FFD0] text-[#53CC6C] text-3xl font-bold size-25 p-2.5 rounded-[50%] flex justify-center items-center mx-auto"
          >
            <h3>01</h3>
          </div>
          <h4 class="text-2xl font-semibold text-[#1C3433]">Contato inicial</h4>
          <p>Preencha o formulário e receba o contato da nossa equipe.</p>
        </li>
        <li class="w-xl relative space-y-8 p-4">
          <NuxtImg
            class="h-14 absolute top-0 right-0 translate-x-1/2"
            src="icons/next-step-icon.svg"
            alt="->"
          />
          <div
            class="bg-[#C4FFD0] text-[#53CC6C] text-3xl font-bold size-25 p-2.5 rounded-[50%] flex justify-center items-center mx-auto"
          >
            <h3>02</h3>
          </div>
          <h4 class="text-2xl font-semibold text-[#1C3433]">
            Briefing Estratégico
          </h4>
          <p>
            Agendamos uma reunião para entender as dores e necessidades da sua
            empresa.
          </p>
        </li>
        <li class="w-xl relative space-y-8 p-4">
          <NuxtImg
            class="h-14 absolute top-0 right-0 translate-x-1/2"
            src="icons/next-step-icon.svg"
            alt="->"
          />
          <div
            class="bg-[#C4FFD0] text-[#53CC6C] text-3xl font-bold size-25 p-2.5 rounded-[50%] flex justify-center items-center mx-auto"
          >
            <h3>03</h3>
          </div>
          <h4 class="text-2xl font-semibold text-[#1C3433]">
            Proposta Personalizada
          </h4>
          <p>Apresentamos um plano estratégico adaptado à sua realidade.</p>
        </li>
        <li class="w-xl relative space-y-8 p-4">
          <NuxtImg
            class="h-14 absolute top-0 right-0 translate-x-1/2"
            src="icons/next-step-icon.svg"
            alt="->"
          />
          <div
            class="bg-[#C4FFD0] text-[#53CC6C] text-3xl font-bold size-25 p-2.5 rounded-[50%] flex justify-center items-center mx-auto"
          >
            <h3>04</h3>
          </div>
          <h4 class="text-2xl font-semibold text-[#1C3433]">
            Onboarding e Planejamento
          </h4>
          <p>Definição do cronograma e estrutura do projeto.</p>
        </li>
      </ul>
      <div class="flex justify-center items-center gap-4">
        <button
          type="button"
          class="bg-[#F7F7F7] rounded-[50%] size-16 flex justify-center items-center cursor-not-allowed"
          disabled
        >
          <NuxtImg src="icons/chevron-left.svg" alt="<-" />
        </button>
        <button
          type="button"
          class="bg-[#F7F7F7] rounded-[50%] size-16 flex justify-center items-center cursor-pointer"
        >
          <NuxtImg src="icons/chevron-right.svg" alt="->" />
        </button>
      </div>
    </section>
    <section class="p-16 space-y-8">
      <h2 class="font-bold text-5xl text-[#1C3433]">
        Para quem é o In Company?
      </h2>
      <div class="flex items-center gap-32">
        <div class="flex-1 space-y-8">
          <p class="font-normal text-lg text-[#6B6A66]">
            Os treinamentos "In Company" são voltados para empresas de diversos
            portes e segmentos que desejam aprimorar seus processos internos,
            capacitar seus colaboradores e fortalecer suas equipes.
          </p>
          <p class="font-normal text-lg text-[#6B6A66]">
            Se sua empresa busca melhorar o desempenho organizacional e garantir
            um ambiente de trabalho mais eficiente e produtivo, esse programa é
            para você.
          </p>
        </div>
        <div class="flex-1">
          <CheckedList
            id="features"
            :items="[
              'Grandes corporações',
              'Instituições de Ensino',
              'Órgãos Públicos',
              'Hospitais e Clínicas',
            ]"
            class-name="grid grid-cols-2 font-semibold"
          />
        </div>
      </div>
    </section>
    <section class="p-32 space-y-16 bg-[#F5F2EC]">
      <h2 class="font-bold text-5xl text-[#1C3433] text-center">
        Serviços mais procurados:
      </h2>
      <ul class="w-full flex items-center justify-center gap-16">
        <li class="w-1/3 space-y-4">
          <NuxtImg src="icons/rocket-icon.svg" alt="Foguete" class="size-12" />
          <h4 class="text-2xl font-semibold text-[#1C3433]">
            Treinamentos e desenvolvimento
          </h4>
          <p class="font-normal text-lg text-[#6B6A66]">
            Capacitação em liderança, vendas, negociação e comunicação.
          </p>
        </li>
        <li class="w-1/3 space-y-4">
          <NuxtImg
            src="icons/megaphone-icon.svg"
            alt="Megafone"
            class="size-12"
          />
          <h4 class="text-2xl font-semibold text-[#1C3433]">
            Consultorias especializadas
          </h4>
          <p class="font-normal text-lg text-[#6B6A66]">
            Diagnóstico e implementação de estratégias em gestão, marketing e
            recursos humanos.
          </p>
        </li>
        <li class="w-1/3 space-y-4">
          <NuxtImg
            src="icons/user-with-tie-icon.svg"
            alt="Corporativo"
            class="size-12"
          />
          <h4 class="text-2xl font-semibold text-[#1C3433]">
            Programas de bem-estar corporativo
          </h4>
          <p class="font-normal text-lg text-[#6B6A66]">
            Técnicas para melhoria do clima organizacional e retenção de
            talentos.
          </p>
        </li>
      </ul>
    </section>
    <section class="p-16 space-y-8">
      <h2 class="font-bold text-5xl text-[#1C3433]">Benefícios In Company?</h2>
      <div class="flex gap-32">
        <div class="flex-1 space-y-8">
          <p class="font-normal text-lg text-[#6B6A66]">
            Investir no treinamento corporativo "In Company" traz vantagens
            diretas para a empresa e seus colaboradores.
          </p>
          <p class="font-normal text-lg text-[#6B6A66]">
            Com uma abordagem personalizada e focada nas reais necessidades do
            seu time, você garante melhorias significativas em diversos aspectos
            organizacionais.
          </p>
        </div>
        <div class="flex-1">
          <ul
            class="space-y-5 text-base text-[#6B6A66] font-medium leading-[170%]"
          >
            <li class="flex space-y-2">
              <div>
                <NuxtImg
                  src="icons/checked-icon.svg"
                  class="size-8 inline-block mr-2"
                />
              </div>
              <div class="w-xl">
                <h6 class="text-[#1C3433] font-bold">Diminuição de Turnove</h6>
                <p>
                  Reduza custos com contratações e treinamentos frequentes,
                  aumentando a retenção de talentos.
                </p>
              </div>
            </li>
            <li class="flex space-y-2">
              <div>
                <NuxtImg
                  src="icons/checked-icon.svg"
                  class="size-8 inline-block mr-2"
                />
              </div>
              <div class="w-xl">
                <h6 class="text-[#1C3433] font-bold">Capacitação da Equipe</h6>
                <p>
                  Desenvolva habilidades estratégicas em liderança, vendas e
                  negociação, tornando seu time mais preparado para desafios do
                  mercado.
                </p>
              </div>
            </li>
            <li class="flex space-y-2">
              <div>
                <NuxtImg
                  src="icons/checked-icon.svg"
                  class="size-8 inline-block mr-2"
                />
              </div>
              <div class="w-xl">
                <h6 class="text-[#1C3433] font-bold">
                  Melhoria do Clima Organizacional
                </h6>
                <p>
                  Fortaleça a cultura da empresa e promova um ambiente de
                  trabalho mais motivador e produtivo.
                </p>
              </div>
            </li>
            <li class="flex space-y-2">
              <div>
                <NuxtImg
                  src="icons/checked-icon.svg"
                  class="size-8 inline-block mr-2"
                />
              </div>
              <div class="w-xl">
                <h6 class="text-[#1C3433] font-bold">Aprimoramento Contínuo</h6>
                <p>
                  Potencialize a performance dos colaboradores com treinamentos
                  práticos e alinhados às necessidades da empresa.
                </p>
              </div>
            </li>
          </ul>
          <!-- <CheckedList
            id="features"
            :items="[
              '',
              'Desenvolva habilidades estratégicas em liderança, vendas e negociação, tornando seu time mais preparado para desafios do mercado.',
              'Melhoria do Clima Organizacional',
              'Fortaleça a cultura da empresa e promova um ambiente de trabalho mais motivador e produtivo.',
              'Aprimoramento Contínuo',
              'Potencialize a performance dos colaboradores com treinamentos práticos e alinhados às necessidades da empresa.',
            ]"
          /> -->
        </div>
      </div>
    </section>
  </main>
  <Footer />
</template>
