<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Promoción Limpieza Dental - Sonrisa Perfecta</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap');
    body { font-family: 'Inter', sans-serif; }
    .gradient-bg { background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); }
    .tooth-icon { animation: bounce 2s infinite; }
    @keyframes bounce {
      0%, 20%, 50%, 80%, 100% { transform: translateY(0); }
      40% { transform: translateY(-10px); }
      60% { transform: translateY(-5px); }
    }
    .shine { position: relative; overflow: hidden; }
    .shine::before {
      content: '';
      position: absolute;
      top: 0; left: -100%;
      width: 100%; height: 100%;
      background: linear-gradient(90deg, transparent, rgba(255,255,255,0.3), transparent);
      animation: shine 3s infinite;
    }
    @keyframes shine {
      0% { left: -100%; }
      100% { left: 100%; }
    }
    .modal {
      display: none;
      position: fixed;
      z-index: 1000;
      left: 0; top: 0;
      width: 100%; height: 100%;
      background-color: rgba(0,0,0,0.5);
    }
    .modal.show {
      display: flex;
      align-items: center;
      justify-content: center;
    }
  </style>
</head>
<body class="bg-gray-50">
  <!-- Header -->
  <header class="gradient-bg text-white py-4">
    <div class="container mx-auto px-4">
      <div class="flex items-center justify-between">
        <div class="flex items-center space-x-3">
          <div class="text-3xl tooth-icon">🦷</div>
          <h1 class="text-2xl font-bold">Moreno Perfect Teeth</h1>
        </div>
        <div class="text-right">
          <p class="text-sm opacity-90">📞 (443) 9339133</p>
          <p class="text-sm opacity-90">📍 Avenida Colegio de San Nicolás, Fray Juan de Zumarraga, 58930 Zinapécuaro de Figueroa, Mich.</p>
        </div>
      </div>
    </div>
  </header>

  <!-- Hero Section -->
  <section class="bg-white py-16">
    <div class="container mx-auto px-4 text-center">
      <div class="max-w-4xl mx-auto">
        <div class="bg-red-500 text-white inline-block px-6 py-2 rounded-full text-sm font-semibold mb-6 animate-pulse">
          ¡OFERTA ESPECIAL POR TIEMPO LIMITADO!
        </div>
        <h2 class="text-5xl font-bold text-gray-800 mb-6">
          Limpieza Dental <span class="text-blue-600">Profesional</span>
        </h2>
        <div class="flex items-center justify-center space-x-4 mb-8">
          <span class="text-4xl text-gray-400 line-through">$800</span>
          <span class="text-6xl font-bold text-green-500">$450</span>
          <div class="bg-yellow-400 text-black px-4 py-2 rounded-lg font-bold">
            ¡AHORRA $350!
          </div>
        </div>
        <p class="text-xl text-gray-600 mb-8 max-w-2xl mx-auto">
          Mantén tu sonrisa radiante con nuestra limpieza dental profesional. Incluye examen completo, limpieza profunda y consejos personalizados.
        </p>
        <button onclick="reservarCita(https://wa.me/qr/P32X4QLYZWTGL1)" class="shine bg-blue-600 hover:bg-blue-700 text-white font-bold py-4 px-8 rounded-full text-xl transition-all duration-300 transform hover:scale-105 shadow-lg">
          🎯 RESERVAR MI CITA AHORA
        </button>
      </div>
    </div>
  </section>

  <!-- Benefits Section -->
  <section class="bg-gray-100 py-16">
    <div class="container mx-auto px-4">
      <h3 class="text-3xl font-bold text-center text-gray-800 mb-12">¿Qué Incluye Tu Limpieza Dental?</h3>
      <div class="grid md:grid-cols-3 gap-8 max-w-6xl mx-auto">
        <div class="bg-white p-8 rounded-lg shadow-lg text-center">
          <div class="text-5xl mb-4">🔍</div>
          <h4 class="text-xl font-semibold text-gray-800 mb-4">Examen Completo</h4>
          <p class="text-gray-600">Revisión detallada de dientes, encías y salud bucal general por nuestros especialistas.</p>
        </div>
        <div class="bg-white p-8 rounded-lg shadow-lg text-center">
          <div class="text-5xl mb-4">✨</div>
          <h4 class="text-xl font-semibold text-gray-800 mb-4">Limpieza Profunda</h4>
          <p class="text-gray-600">Eliminación de placa, sarro y manchas para una sonrisa más blanca y saludable.</p>
        </div>
        <div class="bg-white p-8 rounded-lg shadow-lg text-center">
          <div class="text-5xl mb-4">💡</div>
          <h4 class="text-xl font-semibold text-gray-800 mb-4">Consejos Personalizados</h4>
          <p class="text-gray-600">Recomendaciones específicas para mantener tu higiene bucal en casa.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Testimonials Section -->
  <section class="bg-white py-16">
    <div class="container mx-auto px-4">
      <h3 class="text-3xl font-bold text-center text-gray-800 mb-12">Lo Que Dicen Nuestros Pacientes</h3>
      <div class="grid md:grid-cols-2 gap-8 max-w-4xl mx-auto">
        <div class="bg-blue-50 p-6 rounded-lg">
          <div class="flex items-center mb-4">
            <div class="text-yellow-400 text-xl">⭐⭐⭐⭐⭐</div>
          </div>
          <p class="text-gray-700 mb-4">"Excelente servicio, muy profesionales y mi sonrisa quedó perfecta. Definitivamente regresaré."</p>
          <p class="font-semibold text-gray-800">- María González</p>
        </div>
        <div class="bg-blue-50 p-6 rounded-lg">
          <div class="flex items-center mb-4">
            <div class="text-yellow-400 text-xl">⭐⭐⭐⭐⭐</div>
          </div>
          <p class="text-gray-700 mb-4">"La mejor clínica dental de la zona. Trato amable y resultados increíbles."</p>
          <p class="font-semibold text-gray-800">- Carlos Ramírez</p>
        </div>
      </div>
    </div>
  </section>

  <!-- CTA Section -->
  <section class="gradient-bg py-16">
    <div class="container mx-auto px-4 text-center">
      <div class="max-w-3xl mx-auto text-white">
        <h3 class="text-4xl font-bold mb-6">¡No Esperes Más!</h3>
        <p class="text-xl mb-8 opacity-90">Esta oferta especial es por tiempo limitado. Reserva tu cita hoy y obtén una sonrisa más saludable.</p>
        <div class="flex flex-col sm:flex-row gap-4 justify-center items-center">
          <button onclick="reservarCita()" class="shine bg-white text-blue-600 font-bold py-4 px-8 rounded-full text-xl hover:bg-gray-100 transition-all duration-300 transform hover:scale-105 shadow-lg">
            📞 LLAMAR AHORA
          </button>
          <button onclick="mostrarFormulario()" class="bg-green-500 hover:bg-green-600 text-white font-bold py-4 px-8 rounded-full text-xl transition-all duration-300 transform hover:scale-105 shadow-lg">
            📝 AGENDAR EN LÍNEA
          </button>
        </div>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="bg-gray-800 text-white py-8">
    <div class="container mx-auto px-4">
      <div class="grid md:grid-cols-3 gap-8">
        <div>
          <h4 class="text-xl font-bold mb-4"> MorenoPerfectTeeth</h4>
          <p class="text-gray-300">Tu sonrisa perfecta es nuestra pasión el cuidando la salud bucal de nuestros pacientes.</p>
        </div>
        <div>
          <h4 class="text-xl font-bold mb-4">Contacto</h4>
          <p class="text-gray-300 mb-2">📞 (443) 9339133 (443) 335 4912</p>
          <p class="text-gray-300 mb-2"></p>
          <p class="text-gray-300">📍 Avenida Colegio de San Nicolás, Fray Juan de Zumarraga, 58930 Zinapécuaro de Figueroa, Mich.</p>
        </div>
        <div>
          <h4 class="text-xl font-bold mb-4">Horarios</h4>
          <p class="text-gray-300 mb-2">Lunes - Viernes: 9:00 AM - 7:00 PM</p>
          <p class="text-gray-300 mb-2">Sábados: 9:00 AM - 6:00 PM</p>
          <p class="text-gray-300">Domingos: Cerrado</p>
        </div>
      </div>
      <div class="border-t border-gray-700 mt-8 pt-8 text-center">
        <p class="text-gray-400">&copy; 2025 Moreno Perfect Teeth. Todos los derechos reservados.</p>
      </div>
    </div>
  </footer>

  <!-- Modal for Appointment Form -->
  <div id="appointmentModal" class="modal">
    <div class="bg-white rounded-lg p-8 max-w-md mx-4 w-full">
      <div class="flex justify-between items-center mb-6">
        <h3 class="text-2xl font-bold text-gray-800">Agendar Cita</h3>
        <button onclick="cerrarModal()" class="text-gray-500 hover:text-gray-700 text-2xl">&times;</button>
      </div>
      <form id="appointmentForm" onsubmit="enviarFormulario(event)">
        <div class="mb-4">
          <label class="block text-gray-700 text-sm font-bold mb-2">Nombre Completo</label>
          <input name="nombre" type="text" required class="w-full px-3 py-2 border border-gray-300 rounded-lg focus:outline-none focus:border-blue-500">
        </div>
        <div class="mb-4">
          <label class="block text-gray-700 text-sm font-bold mb-2">Teléfono</label>
          <input name="telefono" type="tel" required class="w-full px-3 py-2 border border-gray-300 rounded-lg focus:outline-none focus:border-blue-500">
        </div>
        <div class="mb-4">
          <label class="block text-gray-700 text-sm font-bold mb-2">Email</label>
          <input name="email" type="email" required class="w-full px-3 py-2 border border-gray-300 rounded-lg focus:outline-none focus:border-blue-500">
        </div>
        <div class="mb-4">
          <label class="block text-gray-700 text-sm font-bold mb-2">Fecha Preferida</label>
          <input name="fecha" type="date" required class="w-full px-3 py-2 border border-gray-300 rounded-lg focus:outline-none focus:border-blue-500">
        </div>
        <div class="mb-6">
          <label class="block text-gray-700 text-sm font-bold mb-2">Hora Preferida</label>
          <select name="hora" required class="w-full px-3 py-2 border border-gray-300 rounded-lg focus:outline-none focus:border-blue-500">
            <option value="">Seleccionar hora</option>
            <option value="09:00">9:00 AM</option>
            <option value="10:00">10:00 AM</option>
            <option value="11:00">11:00 AM</option>
            <option value="12:00">12:00 PM</option>
            <option value="14:00">2:00 PM</option>
            <option value="15:00">3:00 PM</option>
            <option value="16:00">4:00 PM</option>
            <option value="17:00">5:00 PM</option>
          </select>
        </div>
        <button type="submit" class="w-full bg-blue-600 hover:bg-blue-700 text-white font-bold py-3 px-4 rounded-lg transition-colors duration-300">
          Confirmar Cita
        </button>
      </form>
    </div>
  </div>

  <script>
    function reservarCita() {
      // Simulate calling the clinic
      alert('¡Perfecto! Te conectaremos con nuestra recepcionista.\n\nLlama ahora al: (443) 9339133\n\nO usa el botón "AGENDAR EN LÍNEA" para completar tu reserva.');
    }
    function mostrarFormulario() {
      document.getElementById('appointmentModal').classList.add('show');
    }
    function cerrarModal() {
      document.getElementById('appointmentModal').classList.remove('show');
    }
    function enviarFormulario(event) {
      event.preventDefault();
      // Get form data
      const formData = new FormData(event.target);
      const nombre = formData.get('nombre');
      const telefono = formData.get('telefono');
      const email = formData.get('email');
      const fecha = formData.get('fecha');
      const hora = formData.get('hora');
      // Simulate form submission
      alert(`¡Cita agendada exitosamente!\n\nDetalles de tu cita:\n• Nombre: ${nombre}\n• Teléfono: ${telefono}\n• Email: ${email}\n• Fecha: ${fecha}\n• Hora: ${hora}\n\nTe contactaremos pronto para confirmar tu cita. ¡Gracias por elegir Clínica Dental Sonrisa!`);
      // Close modal and reset form
      cerrarModal();
      event.target.reset();
    }
    // Close modal when clicking outside
    document.getElementById('appointmentModal').addEventListener('click', function(e) {
      if (e.target === this) {
        cerrarModal();
      }
    });
  </script>
</body>
</html>
