
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Informe de Revisión Estructural</title>
<style>
body {
  font-family: Arial, sans-serif;
  background: #eef2f6;
  margin: 0;
  padding: 20px;
}
main {
  max-width: 750px;
  margin: auto;
  background: white;
  padding: 25px;
  border-radius: 8px;
}
h1, h2 { color: #17365d; }
label {
  display: block;
  margin-top: 14px;
  font-weight: bold;
}
input, textarea, select {
  box-sizing: border-box;
  width: 100%;
  padding: 10px;
  margin-top: 5px;
  font: inherit;
}
textarea { min-height: 75px; }
button {
  margin-top: 20px;
  padding: 12px;
  background: #17365d;
  color: white;
  border: 0;
  cursor: pointer;
}
@media print {
  body { background: white; padding: 0; }
  main { padding: 0; }
  button { display: none; }
}
</style>
</head>
<body>
<main>
<h1>INFORME DE REVISIÓN ESTRUCTURAL</h1>
<p>Gobierno Autónomo Descentralizado Municipal</p>

<h2>1. Datos generales</h2>

<label>Número de trámite</label>
<input id="tramite" placeholder="Ej. EGOB 123710">

<label>Propietario</label>
<input id="propietario">

<label>Ubicación</label>
<input id="ubicacion">

<label>Tipo de proyecto</label>
<select id="tipo">
  <option value="">Seleccione</option>
  <option>Anteproyecto estructural</option>
  <option>Proyecto estructural definitivo</option>
  <option>Reconocimiento de edificación</option>
</select>

<label>Número de pisos</label>
<input id="pisos" type="number" min="1">

<h2>2. Revisión técnica</h2>

<label>Documentación revisada</label>
<textarea id="documentos"></textarea>

<label>Observaciones</label>
<textarea id="observaciones"></textarea>

<h2>3. Conclusión técnica</h2>
<textarea id="conclusion"></textarea>

<button onclick="window.print()">
Imprimir / Guardar como PDF
</button>
</main>
</body>
</html>
