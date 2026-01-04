# LIBO-crownfounding
LOBI: Simple crowdfunding platform for investors and project owners
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>LOBI | Crowdfunding Platform</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="container">
        <h1>LOBI</h1>
        <p class="subtitle">Simple Crowdfunding Platform</p>

        <div class="buttons">
            <button onclick="showForm('investor')">Investor Login</button>
            <button onclick="showForm('project')">Project Owner Login</button>
        </div>

        <div id="form-area" class="form-area">
            <h2 id="form-title"></h2>
            <input type="email" placeholder="Email">
            <input type="password" placeholder="Password">
            <button class="login-btn">Login</button>
        </div>
    </div>

    <script>
        function showForm(type) {
            const title = document.getElementById('form-title');
            const area = document.getElementById('form-area');
            if (type === 'investor') {
                title.innerText = 'Investor Login';
            } else {
                title.innerText = 'Project Owner Login';
            }
            area.style.display = 'block';
        }
    </script>
</body>
</html>
body {
    margin: 0;
    font-family: Arial, sans-serif;
    background-color: #0f3d2e;
    color: #ffffff;
}

.container {
    max-width: 400px;
    margin: 100px auto;
    background-color: #145a40;
    padding: 30px;
    border-radius: 10px;
    text-align: center;
}

h1 {
    margin-bottom: 5px;
}

.subtitle {
    font-size: 14px;
    margin-bottom: 30px;
    color: #cdeee1;
}

.buttons button {
    width: 100%;
    padding: 12px;
    margin: 10px 0;
    border: none;
    border-radius: 6px;
    background-color: #1e8f66;
    color: white;
    font-size: 16px;
    cursor: pointer;
}

.buttons button:hover {
    background-color: #27ae7a;
}

.form-area {
    display: none;
    margin-top: 20px;
}

.form-area input {
    width: 100%;
    padding: 10px;
    margin: 8px 0;
    border-radius: 5px;
    border: none;
}

.login-btn {
    width: 100%;
    padding: 12px;
    background-color: #0b2f22;
    border: none;
    border-radius: 6px;
    color: white;
    font-size: 16px;
    cursor: pointer;
}

.login-btn:hover {
    background-color: #09271c;
}
