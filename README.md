<!DOCTYPE htlm>
<html lang="fr">

<head>
	<meta charset="UTF-8" />
	<title>Inscription</title>
	<meta charset="">	<meta name="description" content="Inscription"/>

	<body>
		<form action="serveur.php" method="GET">
			<fieldset>	<!-- Les Fieldset ne servent pa à grand chose -->
				<legend>Identité</legend>
				<div>
					<label for="genderm">Homme</label>
					<input type="radio" name="gender" value="m"/>
					<input type="radio" name="gender" value="f">
					<label for="genderf">Femme</label>
				</div>
					<label for="name">Nom</label>
					<input id="name"type="text" name="name">
					<label for="nickname">Prénom</label>
					<input id="nickname"type="text" name="nickname">
				<div>
					<label for="birthdate">Date de naissance</label>
					<input id="birthdate" type="date"/>
				</div>
				<div>
					<label for="homecountry">Pays </label>
					<select id="homecountry" name="homecountry">
						<option value="FRA">France</option>
						<option value="ESP">Espagne</option>
						<option value="ADR">Andorre</option>
					</select>
				</div>
				<div>
					<label for="suggest">Suggestion</label>
					<textarea id="suggest" name="suggest"></textarea>
				</div>
			</fieldset>

		<fieldset>
			<legend>Compte</legend>
				<div>
					<label for="pseudo">Pseudonyme</label>
					<input minlength="3" required id="pseudo" type="text" name="pseudo" placeholder="Pseudonyme" pattern="" value=""/>  <!-- Value n'est pas obligatoire-->
				</div>
				<div>
					<label for="password">Mot de passe</label>
					<input required id="password" type="password" name="password" placeholder="mot de passe"/>
				</div>
				<div>
					<label for="email">Email</label>
					<input id="email" type="email" name="email">
				</div>
		</fieldset>
			<div>
				<input required id="ok" type="checkbox" name="ok">
				<label for="ok"> Je confirme que je confirme</label>
			</div>
			<button style="background-color: greenyellow;" type="submit">S'inscrire </button>
			<button style="background-color: darkred;" type="reset">Annuler</button>
		</form>
	</body>

</head>

</html>
