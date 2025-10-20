<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Vehículos Registrados</title>
<style>
  body {
    font-family: Arial, sans-serif;
    background-color: #f5f6f8;
    margin: 0;
    padding: 20px;
  }

  .container {
    max-width: 750px;
    margin: 0 auto;
  }

  h2 {
    text-align: center;
    margin-bottom: 15px;
  }

  .btn {
    padding: 10px 15px;
    margin: 5px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    color: white;
    background-color: #4169e1;
    font-size: 14px;
  }

  .btn:hover {
    background-color: #27408b;
  }

  .btn-search {
    background-color: #4caf50;
  }

  .btn-search:hover {
    background-color: #357a38;
  }

  .form-container {
    display: none;
    background: white;
    padding: 20px;
    border-radius: 12px;
    margin-bottom: 20px;
    box-shadow: 0 2px 10px rgba(0,0,0,0.1);
  }

  label {
    display: block;
    margin-top: 10px;
    font-weight: bold;
  }

  input {
    width: 100%;
    padding: 8px;
    margin-top: 5px;
    border-radius: 5px;
    border: 1px solid #ccc;
    box-sizing: border-box;
  }

  table {
    width: 100%;
    border-collapse: collapse;
    margin-top: 10px;
  }

  th, td {
    border-bottom: 1px solid #ddd;
    padding: 8px;
    text-align: left;
    font-size: 14px;
  }

  th {
    background-color: #f0f2f5;
  }
</style>
</head>
<body>

<div class="container">
  <h2>🚗 Vehículos Registrados (Civiles)</h2>

  <!-- Botones -->
  <div style="text-align:center;">
    <button class="btn" id="btnRegistrar">Registrar vehículo</button>
    <button class="btn btn-search" id="btnBuscar">🔍 Buscar vehículo</button>
  </div>

  <!-- Formulario -->
  <div class="form-container" id="formVehiculo">
    <h3>Formulario de vehículo</h3>

    <label>RUT:</label>
    <input type="text" id="rut" placeholder="Ej: 12345678-9" required>

    <label>Nombre:</label>
    <input type="text" id="nombre" placeholder="Nombre del propietario" required>

    <label>Placa:</label>
    <input type="text" id="placa" placeholder="Ej: ABC123" required>

    <label>Marca:</label>
    <input type="text" id="marca" placeholder="Ej: Toyota" required>

    <label>Modelo:</label>
    <input type="text" id="modelo" placeholder="Ej: Yaris" required>

    <label>Color:</label>
    <input type="text" id="color" placeholder="Ej: Blanco" required>

    <label>Año:</label>
    <input type="number" id="anio" placeholder="Ej: 2020" required>

    <button class="btn" id="guardarVehiculo">Guardar vehículo</button>
  </div>

  <!-- Tabla -->
  <table id="tablaVehiculos">
    <tr>
      <th>RUT</th>
      <th>Nombre</th>
      <th>P.P.U</th>
      <th>Marca</th>
      <th>Modelo</th>
      <th>Color</th>
      <th>Año</th>
    </tr>
  </table>
</div>

<script>
const btnRegistrar = document.getElementById("btnRegistrar");
const btnBuscar = document.getElementById("btnBuscar");
const formVehiculo = document.getElementById("formVehiculo");
const tabla = document.getElementById("tablaVehiculos");

// Función para actualizar la tabla
function actualizarTabla(filtro = "") {
  const vehiculos = JSON.parse(localStorage.getItem("vehiculos")) || [];
  tabla.innerHTML = `
    <tr>
      <th>RUT</th>
      <th>Nombre</th>
      <th>P.P.U</th>
      <th>Marca</th>
      <th>Modelo</th>
      <th>Color</th>
      <th>Año</th>
    </tr>
  `;
  vehiculos
    .filter(v => v.placa.includes(filtro) || v.modelo.toLowerCase().includes(filtro.toLowerCase()) || v.rut.includes(filtro) || v.nombre.toLowerCase().includes(filtro.toLowerCase()))
    .forEach(v => {
      const fila = tabla.insertRow(-1);
      fila.insertCell(0).innerText = v.rut;
      fila.insertCell(1).innerText = v.nombre;
      fila.insertCell(2).innerText = v.placa;
      fila.insertCell(3).innerText = v.marca;
      fila.insertCell(4).innerText = v.modelo;
      fila.insertCell(5).innerText = v.color;
      fila.insertCell(6).innerText = v.anio;
    });
}

// Mostrar formulario solo con clave correcta
btnRegistrar.addEventListener("click", () => {
  const clave = prompt("Ingrese la clave para registrar vehículo:");
  if(clave === "Estrella2010") {
    formVehiculo.style.display = "block";
    formVehiculo.scrollIntoView({ behavior: "smooth" });
  } else {
    alert("Clave incorrecta.");
  }
});

// Guardar vehículo
document.getElementById("guardarVehiculo").addEventListener("click", () => {
  const rut = document.getElementById("rut").value.trim();
  const nombre = document.getElementById("nombre").value.trim();
  const placa = document.getElementById("placa").value.trim();
  const marca = document.getElementById("marca").value.trim();
  const modelo = document.getElementById("modelo").value.trim();
  const color = document.getElementById("color").value.trim();
  const anio = document.getElementById("anio").value.trim();

  if(!rut || !nombre || !placa || !marca || !modelo || !color || !anio) {
    alert("Por favor, complete todos los campos.");
    return;
  }

  const vehiculos = JSON.parse(localStorage.getItem("vehiculos")) || [];
  vehiculos.push({ rut, nombre, placa, marca, modelo, color, anio });
  localStorage.setItem("vehiculos", JSON.stringify(vehiculos));

  // Limpiar formulario
  document.getElementById("rut").value = "";
  document.getElementById("nombre").value = "";
  document.getElementById("placa").value = "";
  document.getElementById("marca").value = "";
  document.getElementById("modelo").value = "";
  document.getElementById("color").value = "";
  document.getElementById("anio").value = "";

  actualizarTabla();
  formVehiculo.style.display = "none";
  tabla.scrollIntoView({ behavior: "smooth" });
});

// Buscar vehículo
btnBuscar.addEventListener("click", () => {
  const busqueda = prompt("Ingrese RUT, placa, nombre o modelo a buscar:");
  actualizarTabla(busqueda || "");
});

// Cargar tabla al iniciar
actualizarTabla();
</script>

</body>
</html>
