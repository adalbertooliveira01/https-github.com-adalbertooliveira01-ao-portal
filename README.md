# https-github.com-adalbertooliveira01-ao-portal
app/
components/
public/
styles/
lib/
import Header from "@/components/Header";
import Hero from "@/components/Hero";
import Footer from "@/components/Footer";

export default function Home() {
  return (
    <>
      <Header />
      <Hero />

      <main className="max-w-7xl mx-auto px-6 py-20">

        <section className="grid md:grid-cols-2 lg:grid-cols-4 gap-6">

          <div className="rounded-xl shadow-lg p-6">
            <h2 className="text-2xl font-bold">📘 Educação</h2>
            <p>Projetos, cursos e materiais.</p>
          </div>

          <div className="rounded-xl shadow-lg p-6">
            <h2 className="text-2xl font-bold">🏛 Gestão Pública</h2>
            <p>Consultoria e planejamento.</p>
          </div>

          <div className="rounded-xl shadow-lg p-6">
            <h2 className="text-2xl font-bold">🏭 Engenharia</h2>
            <p>Projetos industriais.</p>
          </div>

          <div className="rounded-xl shadow-lg p-6">
            <h2 className="text-2xl font-bold">🤖 Inteligência Artificial</h2>
            <p>Pesquisa e inovação.</p>
          </div>

        </section>

      </main>

      <Footer />
    </>
  );
}
export default function Header() {
  return (
    <header className="bg-[#0A2342] text-white">

      <div className="max-w-7xl mx-auto flex justify-between items-center p-6">

        <h1 className="text-2xl font-bold">
          Adalberto Oliveira
        </h1>

        <nav className="space-x-8">

          <a href="#">Início</a>

          <a href="#">Sobre</a>

          <a href="#">Educação</a>

          <a href="#">Gestão</a>

          <a href="#">Engenharia</a>

          <a href="#">IA</a>

          <a href="#">Contato</a>

        </nav>

      </div>

    </header>
  );
}
export default function Hero() {
  return (

<section className="bg-[#0A2342] text-white py-32">

<div className="max-w-7xl mx-auto px-6">

<h1 className="text-6xl font-bold">

Prof. Adalberto Olimpio de Oliveira

</h1>

<p className="text-2xl mt-6">

Consultor Técnico Multidisciplinar

</p>

<p className="mt-10 text-xl">

Educação • Gestão Pública • Engenharia • Inteligência Artificial

</p>

<div className="mt-12">

<button className="bg-yellow-500 text-black px-8 py-4 rounded-lg mr-5">

Conheça minha história

</button>

<button className="border border-white px-8 py-4 rounded-lg">

Biblioteca

</button>

</div>

</div>

</section>

  );
}
export default function Footer() {

return (

<footer className="bg-[#0A2342] text-white py-10">

<div className="max-w-7xl mx-auto text-center">

© 2026

Prof. Adalberto Olimpio de Oliveira

</div>

</footer>

);

}
┌──────────────────────────────────────────┐
│ Header (fixo)                            │
├──────────────────────────────────────────┤
│ Hero (imagem + apresentação)             │
├──────────────────────────────────────────┤
│ Indicadores                              │
├──────────────────────────────────────────┤
│ Áreas de atuação                         │
├──────────────────────────────────────────┤
│ Linha do tempo                           │
├──────────────────────────────────────────┤
│ Biblioteca Digital                       │
├──────────────────────────────────────────┤
│ Chamada para contato                     │
├──────────────────────────────────────────┤
│ Footer                                   │
└──────────────────────────────────────────┘
+30
Anos de experiência

3
Licenciaturas

10+
Especializações

100+
Cursos e Certificações
AO Portal
│
├── app
│
├── components
│     ├── layout
│     ├── sections
│     ├── ui
│     ├── cards
│     └── common
│
├── data
│
├── hooks
│
├── lib
│
├── public
│
├── services
│
├── types
│
└── utils
components/ui
interface Props {
  title: string;
  subtitle?: string;
}

export default function SectionTitle({
  title,
  subtitle,
}: Props) {
  return (
    <div className="mb-12">

      <h2 className="text-4xl font-bold text-[#0A2342]">
        {title}
      </h2>

      {subtitle && (
        <p className="text-gray-600 mt-3 text-lg">
          {subtitle}
        </p>
      )}

    </div>
  );
}
components/cards
interface Props{
    emoji:string
    titulo:string
    descricao:string
}

export default function AreaCard({
emoji,
titulo,
descricao
}:Props){

return(

<div className="rounded-xl bg-white shadow-lg hover:shadow-2xl transition-all p-8">

<div className="text-5xl">

{emoji}

</div>

<h3 className="text-2xl font-bold mt-6">

{titulo}

</h3>

<p className="mt-4 text-gray-600">

{descricao}

</p>

<button className="mt-8 bg-[#0A2342] text-white px-5 py-3 rounded-lg hover:bg-[#13396c]">

Saiba mais

</button>

</div>

)

}
className="bg-gradient-to-r from-[#07182E] via-[#0A2342] to-[#123D72]"
