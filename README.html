<!DOCTYPE html>
<html>
<head>
  <title>Tabla de Registro</title>
  <style>
    table {
      border-collapse: collapse;
      width: 100%;
    }
    th, td {
      border: 1px solid black;
      padding: 8px;
      text-align: center;
    }
    th {
      background-color: lightgray;
    }
    td.empty {
      background-color: white;
      cursor: pointer;
    }
    td.registered {
      cursor: not-allowed;
    }
  </style>
</head>
<body>
  <h1>Horarios Canal</h1>
  <table>
    <tr>
      <th>Hora</th>
      <th>Lunes</th>
      <th>Martes</th>
      <th>Miércoles</th>
      <th>Jueves</th>
      <th>Viernes</th>
      <th>Sábado</th>
      <th>Domingo</th>
    </tr>

    <!-- JavaScript loop to generate rows for each hour -->
    <script>
      var hours = ['10 a.m.', '11 a.m.', '12 p.m.', '1 p.m.', '2 p.m.', '3 p.m.', '4 p.m.', '5 p.m.', '6 p.m.', '7 p.m.'];
      var days = ['Lunes', 'Martes', 'Miércoles', 'Jueves', 'Viernes','Sábado','Domingo'];

      // Load stored registrations from local storage or initialize an empty object
      var registrations = JSON.parse(localStorage.getItem('registrations')) || {};

      // Remove registrations older than 24 hours
      for (var key in registrations) {
        if (registrations.hasOwnProperty(key)) {
          var registrationTime = new Date(registrations[key].timestamp);
          var currentTime = new Date();

          // Calculate the time difference in milliseconds
          var timeDiff = currentTime - registrationTime;

          // Convert milliseconds to hours
          var hoursDiff = timeDiff / (1000 * 60 * 60);

          if (hoursDiff >= 24) {
            delete registrations[key];
          }
        }
      }

      for (var i = 0; i < hours.length; i++) {
        document.write('<tr>');
        document.write('<td>' + hours[i] + '</td>');

        for (var j = 0; j < days.length; j++) {
          var key = days[j] + hours[i];

          if (registrations.hasOwnProperty(key)) {
            var registration = registrations[key];
            var content = '<strong>' + registration.name + '</strong><br>' + registration.numPalistas;
            document.write('<td class="registered" style="background-color: green; color: white;">' + content + '</td>');
          } else {
            document.write('<td class="empty" onclick="register(\'' + days[j] + '\', \'' + hours[i] + '\', this)"></td>');
          }
        }

        document.write('</tr>');
      }

      // Save registrations to local storage
      localStorage.setItem('registrations', JSON.stringify(registrations));
    </script>

  </table>

  <script>
    function register(day, hour, cell) {
      var name = prompt("Ingresa tu nombre:");
      if (name) {
        var numPalistas = prompt("Ingresa el número de palistas:");
        if (numPalistas) {
          var content = '<strong>' + name + '</strong><br>' + numPalistas;
          cell.innerHTML = content;
          cell.classList.remove("empty");
          cell.classList.add("registered");
          cell.style.backgroundColor = "green";
          cell.style.color = "white";

          var randomNumber = Math.floor(Math.random() * 100);
          alert("El número de tus dorsales es: " + randomNumber.toString().padStart(2, '0'));

          var key = day + hour;
          var registration = {
            name: name,
            numPalistas: numPalistas,
            timestamp: new Date().toISOString()
          };

          // Store the registration with the key as the day and hour combination
          registrations[key] = registration;

          // Save registrations to local storage
          localStorage.setItem('registrations', JSON.stringify(registrations));
        }
      }
    }
  </script>
</body>
</html>

