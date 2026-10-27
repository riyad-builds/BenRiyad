## Hi there 👋


- a ML enthusiast that's trying to make a legend out of his story.



"/*<?php
$host = '192.168.56.101';
$username = 'remote_user';
$password = 'votre_mot_de_passe';
$database = 'mysql';

$conn = new mysqli($host, $username, $password, $database);

if ($conn->connect_error) {
    die("Erreur de connexion : " . $conn->connect_error);
}

$sql = "SELECT User, Host FROM user";
$result = $conn->query($sql);

echo "<h1>Résultat de la requête depuis MV02</h1>";
if ($result->num_rows > 0) {
    echo "<table border='1'><tr><th>User</th><th>Host</th></tr>";
    while($row = $result->fetch_assoc()) {
        echo "<tr><td>" . $row["User"]. "</td><td>" . $row["Host"]. "</td></tr>";
    }
    echo "</table>";
} else {
    echo "0 résultats";
}
$conn->close();
?>
*/"
