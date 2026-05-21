# Hi
export default function DownloadAnyWebsite() { return ( <div className="min-h-screen bg-gray-100 text-gray-900"> <header className="bg-black text-white p-6 shadow-lg"> <div className="max-w-6xl mx-auto flex items-center justify-between"> <h1 className="text-3xl font-bold">Download Any</h1> <nav className="space-x-4 text-sm"> <a href="#home" className="hover:text-gray-300">Home</a> <a href="#downloads" className="hover:text-gray-300">Downloads</a> <a href="#about" className="hover:text-gray-300">About</a> <a href="#contact" className="hover:text-gray-300">Contact</a> </nav> </div> </header>

<section id="home" className="max-w-6xl mx-auto px-6 py-16 text-center">
    <h2 className="text-5xl font-bold mb-4">Download Apps, Games & Files Easily</h2>
    <p className="text-lg text-gray-600 mb-8">
      Fast, secure and simple downloads with Download Any.
    </p>

    <div className="max-w-2xl mx-auto flex gap-3">
      <input
        type="text"
        placeholder="Search apps, games or files..."
        className="flex-1 p-4 rounded-2xl border border-gray-300 shadow-sm"
      />
      <button className="bg-black text-white px-6 rounded-2xl hover:bg-gray-800">
        Search
      </button>
    </div>
  </section>

  <section id="downloads" className="max-w-6xl mx-auto px-6 pb-16">
    <h3 className="text-3xl font-bold mb-8">Popular Downloads</h3>

    <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
      {[
        {
          title: 'Video Editor Pro',
          category: 'Editing App',
        },
        {
          title: 'Mobile Racing Game',
          category: 'Android Game',
        },
        {
          title: 'Photo Background Remover',
          category: 'AI Tool',
        },
      ].map((item, index) => (
        <div
          key={index}
          className="bg-white rounded-3xl p-6 shadow-md hover:shadow-xl transition"
        >
          <div className="h-40 bg-gray-200 rounded-2xl mb-4"></div>
          <h4 className="text-2xl font-semibold mb-2">{item.title}</h4>
          <p className="text-gray-500 mb-4">{item.category}</p>
          <button className="w-full bg-black text-white py-3 rounded-2xl hover:bg-gray-800">
            Download
          </button>
        </div>
      ))}
    </div>
  </section>

  <section id="about" className="bg-white py-16 px-6">
    <div className="max-w-4xl mx-auto text-center">
      <h3 className="text-3xl font-bold mb-4">About Download Any</h3>
      <p className="text-gray-600 text-lg leading-relaxed">
        Download Any is a modern download platform where users can find apps,
        tools, games and useful resources quickly and securely.
      </p>
    </div>
  </section>

  <section id="contact" className="py-16 px-6 text-center">
    <h3 className="text-3xl font-bold mb-4">Contact Us</h3>
    <p className="text-gray-600 mb-6">support@downloadany.com</p>
    <button className="bg-black text-white px-8 py-3 rounded-2xl hover:bg-gray-800">
      Send Message
    </button>
  </section>

  <footer className="bg-black text-white py-6 text-center">
    <p>© 2026 Download Any. All rights reserved.</p>
  </footer>
</div>

); }
