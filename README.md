export default function EpicesPlusWebsite() { return ( <div className="min-h-screen bg-gradient-to-b from-red-950 via-orange-950 to-amber-950 text-white font-sans"> {/* HERO SECTION */} <section className="relative overflow-hidden px-6 py-20 lg:px-20"> <div className="absolute inset-0 opacity-20 bg-[url('https://images.unsplash.com/photo-1504674900247-0877df9cc836')] bg-cover bg-center"></div>

<div className="relative z-10 max-w-7xl mx-auto grid lg:grid-cols-2 gap-12 items-center">
      <div>
        <div className="inline-block px-4 py-2 rounded-full bg-red-600/30 border border-red-400 mb-6">
          <p className="text-sm tracking-widest uppercase">
            Saveurs Africaines Premium
          </p>
        </div>

        <h1 className="text-5xl lg:text-7xl font-black leading-tight">
          ÉPICES <span className="text-orange-400">PLUS</span>
        </h1>

        <p className="mt-6 text-xl text-orange-100 leading-relaxed max-w-2xl">
          Les meilleures épices d’assaisonnement africaines pour une cuisine saine, rapide et savoureuse.
          Remplacez les cubes industriels par des saveurs naturelles riches en goût.
        </p>

        <div className="mt-10 flex flex-wrap gap-4">
          <a
            href="https://wa.me/2290150802835"
            className="px-8 py-4 rounded-2xl bg-red-600 hover:bg-red-500 transition text-lg font-bold shadow-2xl"
          >
            Commander Maintenant
          </a>

          <a
            href="#products"
            className="px-8 py-4 rounded-2xl border border-orange-300 hover:bg-orange-400 hover:text-black transition text-lg font-semibold"
          >
            Découvrir Nos Produits
          </a>
        </div>
      </div>

      <div className="relative">
        <div className="rounded-[40px] overflow-hidden shadow-[0_0_60px_rgba(255,80,0,0.4)] border border-orange-400/30">
          <img
            src="https://images.unsplash.com/photo-1502741338009-cac2772e18bc?q=80&w=1200&auto=format&fit=crop"
            alt="Épices africaines"
            className="w-full h-[600px] object-cover"
          />
        </div>
      </div>
    </div>
  </section>

  {/* FEATURES */}
  <section className="px-6 lg:px-20 py-20">
    <div className="max-w-7xl mx-auto grid md:grid-cols-3 gap-8">
      {[
        {
          title: '100% Naturel',
          text: 'Des ingrédients naturels sélectionnés pour une cuisine plus saine.'
        },
        {
          title: 'Cuisine Rapide',
          text: 'Préparez des plats savoureux rapidement sans cubes industriels.'
        },
        {
          title: 'Saveurs Africaines',
          text: 'Le goût authentique des cuisines africaines modernes.'
        }
      ].map((item, index) => (
        <div
          key={index}
          className="bg-white/5 backdrop-blur-md border border-orange-500/20 rounded-3xl p-8 hover:scale-105 transition duration-300 shadow-xl"
        >
          <h3 className="text-2xl font-bold text-orange-300 mb-4">
            {item.title}
          </h3>
          <p className="text-orange-100 leading-relaxed">
            {item.text}
          </p>
        </div>
      ))}
    </div>
  </section>

  {/* PRODUCTS */}
  <section id="products" className="px-6 lg:px-20 py-20 bg-black/20">
    <div className="max-w-7xl mx-auto">
      <div className="text-center mb-16">
        <h2 className="text-5xl font-black mb-6 text-orange-300">
          Nos Produits Premium
        </h2>
        <p className="text-orange-100 max-w-3xl mx-auto text-lg">
          Découvrez des produits naturels conçus pour remplacer les cubes de cuisine et améliorer votre santé.
        </p>
      </div>

      <div className="grid md:grid-cols-2 lg:grid-cols-4 gap-8">
        {[
          {
            title: 'Épices d’Assaisonnement',
            image: 'https://images.unsplash.com/photo-1532336414038-cf19250c5757?q=80&w=1000&auto=format&fit=crop'
          },
          {
            title: 'Piment de Table',
            image: 'https://images.unsplash.com/photo-1512621776951-a57141f2eefd?q=80&w=1000&auto=format&fit=crop'
          },
          {
            title: 'Crevettes Moulues',
            image: 'https://images.unsplash.com/photo-1565680018434-b513d5e5fd47?q=80&w=1000&auto=format&fit=crop'
          },
          {
            title: 'Crabe & Poisson Moulu',
            image: 'https://images.unsplash.com/photo-1544025162-d76694265947?q=80&w=1000&auto=format&fit=crop'
          }
        ].map((product, index) => (
          <div
            key={index}
            className="bg-white/5 border border-orange-500/20 rounded-[30px] overflow-hidden hover:scale-105 transition duration-300 shadow-2xl"
          >
            <img
              src={product.image}
              alt={product.title}
              className="h-72 w-full object-cover"
            />

            <div className="p-6">
              <h3 className="text-2xl font-bold text-orange-300 mb-4">
                {product.title}
              </h3>

              <button className="w-full py-3 rounded-xl bg-red-600 hover:bg-red-500 transition font-bold text-lg">
                Commander
              </button>
            </div>
          </div>
        ))}
      </div>
    </div>
  </section>

  {/* ABOUT */}
  <section className="px-6 lg:px-20 py-20">
    <div className="max-w-7xl mx-auto grid lg:grid-cols-2 gap-16 items-center">
      <div>
        <img
          src="https://images.unsplash.com/photo-1504674900247-0877df9cc836?q=80&w=1200&auto=format&fit=crop"
          alt="Cuisine africaine"
          className="rounded-[40px] shadow-2xl"
        />
      </div>

      <div>
        <h2 className="text-5xl font-black text-orange-300 mb-8">
          Une Nouvelle Façon de Cuisiner
        </h2>

        <p className="text-lg text-orange-100 leading-relaxed mb-6">
          ÉPICES PLUS aide les familles à cuisiner plus sainement avec des produits naturels riches en goût.
        </p>

        <p className="text-lg text-orange-100 leading-relaxed mb-6">
          Nos épices et assaisonnements remplacent les cubes industriels souvent nocifs pour la santé.
        </p>

        <p className="text-lg text-orange-100 leading-relaxed">
          Notre mission est de valoriser la cuisine africaine moderne avec des saveurs authentiques et premium.
        </p>
      </div>
    </div>
  </section>

  {/* CONTACT */}
  <section className="px-6 lg:px-20 py-20 bg-gradient-to-r from-red-900 to-orange-800">
    <div className="max-w-5xl mx-auto text-center">
      <h2 className="text-5xl font-black mb-8">
        Passez Votre Commande
      </h2>

      <p className="text-xl text-orange-100 mb-10">
        Commandez directement en ligne ou contactez-nous sur WhatsApp.
      </p>

      <a
        href="https://wa.me/2290150802835"
        className="inline-block px-10 py-5 rounded-2xl bg-white text-red-700 font-black text-xl hover:scale-105 transition shadow-2xl"
      >
        WhatsApp : +229 01 50 80 28 35
      </a>
    </div>
  </section>

  {/* FOOTER */}
  <footer className="py-10 text-center border-t border-orange-500/20 bg-black/40">
    <h3 className="text-3xl font-black text-orange-300 mb-3">
      ÉPICES PLUS
    </h3>

    <p className="text-orange-100">
      Cuisine saine • Saveurs naturelles • Luxe africain
    </p>
  </footer>
</div>

); }
