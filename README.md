export default function BakhliStudioWebsite() {
  return (
    <div className="bg-black text-white min-h-screen font-sans">
      {/* Navbar */}
      <nav className="flex items-center justify-between px-8 py-6 border-b border-zinc-800 sticky top-0 bg-black/90 backdrop-blur z-50">
        <div>
          <h1 className="text-3xl font-bold tracking-wide text-yellow-500">BAKHLI STUDIO</h1>
          <p className="text-sm text-zinc-400 tracking-[4px]">LUXURY WITH TRADITION</p>
        </div>

        <div className="hidden md:flex gap-8 text-sm uppercase tracking-widest text-zinc-300">
          <a href="#about" className="hover:text-yellow-500 transition">About</a>
          <a href="#services" className="hover:text-yellow-500 transition">Services</a>
          <a href="#projects" className="hover:text-yellow-500 transition">Projects</a>
          <a href="#contact" className="hover:text-yellow-500 transition">Contact</a>
        </div>
      </nav>

      {/* Hero Section */}
      <section className="relative h-screen flex items-center justify-center text-center px-6 overflow-hidden">
        <div className="absolute inset-0 bg-[url('https://images.unsplash.com/photo-1505693416388-ac5ce068fe85?q=80&w=2070')] bg-cover bg-center opacity-30"></div>
        <div className="absolute inset-0 bg-gradient-to-b from-black/50 via-black/70 to-black"></div>

        <div className="relative z-10 max-w-4xl">
          <h1 className="text-5xl md:text-7xl font-bold leading-tight mb-6">
            Luxury Hardware <br />
            <span className="text-yellow-500">& Smart Spaces</span>
          </h1>

          <p className="text-zinc-300 text-lg md:text-xl mb-8 leading-relaxed">
            Sliding Partition Systems • Wardrobe Hardware • Kitchen Hardware • Door Solutions
          </p>

          <div className="flex flex-col md:flex-row justify-center gap-4">
            <button className="bg-yellow-500 text-black px-8 py-4 rounded-full font-semibold hover:scale-105 transition">
              Explore Projects
            </button>

            <button className="border border-yellow-500 text-yellow-500 px-8 py-4 rounded-full font-semibold hover:bg-yellow-500 hover:text-black transition">
              Book Consultation
            </button>
          </div>
        </div>
      </section>

      {/* About */}
      <section id="about" className="py-24 px-8 md:px-20 bg-zinc-950">
        <div className="grid md:grid-cols-2 gap-14 items-center">
          <div>
            <h2 className="text-4xl font-bold mb-6 text-yellow-500">About Bakhli Studio</h2>
            <p className="text-zinc-300 leading-8 text-lg">
              Bakhli Studio blends luxury architectural hardware with smart space solutions.
              We create modern, functional, and timeless interiors using premium fittings,
              concealed systems, and luxury design concepts.
            </p>

            <div className="mt-8 grid grid-cols-2 gap-4">
              <div className="border border-zinc-800 rounded-2xl p-6 bg-black">
                <h3 className="text-3xl font-bold text-yellow-500">100+</h3>
                <p className="text-zinc-400 mt-2">Luxury Concepts</p>
              </div>

              <div className="border border-zinc-800 rounded-2xl p-6 bg-black">
                <h3 className="text-3xl font-bold text-yellow-500">Premium</h3>
                <p className="text-zinc-400 mt-2">Hardware Solutions</p>
              </div>
            </div>
          </div>

          <div>
            <img
              src="https://images.unsplash.com/photo-1484154218962-a197022b5858?q=80&w=2070"
              alt="Luxury Interior"
              className="rounded-3xl shadow-2xl border border-zinc-800"
            />
          </div>
        </div>
      </section>

      {/* Services */}
      <section id="services" className="py-24 px-8 md:px-20 bg-black">
        <div className="text-center mb-16">
          <h2 className="text-5xl font-bold text-yellow-500 mb-4">Our Services</h2>
          <p className="text-zinc-400 text-lg">Premium Solutions For Luxury Living</p>
        </div>

        <div className="grid md:grid-cols-2 lg:grid-cols-4 gap-8">
          {[
            {
              title: 'Sliding Partition Systems',
              desc: 'Concealed sliding & folding systems for modern interiors.'
            },
            {
              title: 'Luxury Wardrobe Hardware',
              desc: 'Premium fittings, organizers & wardrobe accessories.'
            },
            {
              title: 'Kitchen Hardware',
              desc: 'Smart storage, lift-up systems & soft-close solutions.'
            },
            {
              title: 'Door Hardware',
              desc: 'Concealed hinges, pivot systems & luxury fittings.'
            }
          ].map((service, index) => (
            <div
              key={index}
              className="border border-zinc-800 bg-zinc-950 p-8 rounded-3xl hover:border-yellow-500 transition hover:-translate-y-2"
            >
              <h3 className="text-2xl font-semibold mb-4 text-yellow-500">{service.title}</h3>
              <p className="text-zinc-400 leading-7">{service.desc}</p>
            </div>
          ))}
        </div>
      </section>

      {/* Projects */}
      <section id="projects" className="py-24 px-8 md:px-20 bg-zinc-950">
        <div className="text-center mb-16">
          <h2 className="text-5xl font-bold text-yellow-500 mb-4">Featured Projects</h2>
          <p className="text-zinc-400 text-lg">Luxury Spaces Crafted With Precision</p>
        </div>

        <div className="grid md:grid-cols-3 gap-8">
          {[
            'https://images.unsplash.com/photo-1615874959474-d609969a20ed?q=80&w=1200',
            'https://images.unsplash.com/photo-1600566752355-35792bedcfea?q=80&w=1200',
            'https://images.unsplash.com/photo-1600585154526-990dced4db0d?q=80&w=1200'
          ].map((img, index) => (
            <div key={index} className="overflow-hidden rounded-3xl border border-zinc-800 group">
              <img
                src={img}
                alt="Project"
                className="h-[400px] w-full object-cover group-hover:scale-110 transition duration-700"
              />
            </div>
          ))}
        </div>
      </section>

      {/* Why Choose Us */}
      <section className="py-24 px-8 md:px-20 bg-black text-center">
        <h2 className="text-5xl font-bold text-yellow-500 mb-14">Why Choose Us</h2>

        <div className="grid md:grid-cols-3 gap-8">
          {[
            'Premium Global Hardware',
            'Architect Friendly Solutions',
            'Luxury Design Concepts',
            'Site Support & Consultation',
            'Modern Smart Space Planning',
            'Trusted Project Execution'
          ].map((item, index) => (
            <div
              key={index}
              className="border border-zinc-800 rounded-3xl p-8 bg-zinc-950 text-lg hover:border-yellow-500 transition"
            >
              {item}
            </div>
          ))}
        </div>
      </section>

      {/* Contact */}
      <section id="contact" className="py-24 px-8 md:px-20 bg-zinc-950">
        <div className="max-w-4xl mx-auto text-center">
          <h2 className="text-5xl font-bold text-yellow-500 mb-6">Let's Build Luxury Together</h2>

          <p className="text-zinc-400 text-lg leading-8 mb-10">
            DM for Projects, Collaborations & Luxury Space Solutions.
          </p>

          <div className="flex flex-col md:flex-row gap-4 justify-center">
            <button className="bg-yellow-500 text-black px-8 py-4 rounded-full font-semibold hover:scale-105 transition">
              WhatsApp Us
            </button>

            <a
              href="https://www.instagram.com/bakhli.studio/"
              target="_blank"
              rel="noopener noreferrer"
              className="border border-yellow-500 text-yellow-500 px-8 py-4 rounded-full font-semibold hover:bg-yellow-500 hover:text-black transition inline-flex items-center justify-center cursor-pointer"
            >
              Instagram Page
            </a>
          </div>
        </div>
      </section>

      {/* Footer */}
      <footer className="border-t border-zinc-800 py-8 text-center text-zinc-500 text-sm tracking-widest">
        © 2026 BAKHLI STUDIO • LUXURY WITH TRADITION
      </footer>
    </div>
  )
}
