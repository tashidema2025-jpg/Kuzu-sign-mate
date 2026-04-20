<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sign Mate | Business Portal</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

<div class="login-container">
    <div class="brand-side">
        <h1>Sign Mate</h1>
        <p>Empowering communication through professional AI sign recognition.</p>
    </div>

    <div class="form-side">
        <form id="login-form">
            <h2>Welcome Back</h2>
            <p>Please enter your details to continue.</p>

            <div class="input-group">
                <label>Email Address</label>
                <input type="email" placeholder="e.g. name@company.com" required>
            </div>

            <div class="input-group">
                <label>Password</label>
                <input type="password" placeholder="••••••••" required>
            </div>

            <div class="form-options">
                <a href="#" class="forgot-link">Forgot password?</a>
            </div>

            <button type="submit" class="btn-primary">Sign In</button>

            <div class="divider">or</div>

            <button type="button" class="btn-google">
                <img src="https://upload.wikimedia.org/wikipedia/commons/c/c1/Google_Reference_Icon.svg" alt="Google">
                Continue with Google
            </button>
        </form>
    </div>
</div>

</body>
</html>
2. Business Style CSS (style.css)
This will give it that high-end, corporate software look (clean borders, subtle shadows, and professional blue).

CSS
:root {
    --primary: #0056b3;
    --dark: #1a1a1b;
    --grey: #6c757d;
    --light-bg: #f8f9fa;
}

body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    margin: 0;
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100vh;
    background-color: var(--light-bg);
}

.login-container {
    display: flex;
    width: 900px;
    height: 550px;
    background: white;
    box-shadow: 0 10px 30px rgba(0,0,0,0.1);
    border-radius: 12px;
    overflow: hidden;
}

/* Left Panel */
.brand-side {
    flex: 1;
    background: var(--primary);
    color: white;
    padding: 60px;
    display: flex;
    flex-direction: column;
    justify-content: center;
}

.brand-side h1 { font-size: 2.5rem; margin-bottom: 20px; }

/* Right Panel */
.form-side {
    flex: 1.2;
    padding: 60px;
}

h2 { color: var(--dark); margin-bottom: 5px; }
p { color: var(--grey); margin-bottom: 30px; font-size: 0.9rem; }

.input-group { margin-bottom: 20px; text-align: left; }
.input-group label { display: block; font-size: 0.85rem; font-weight: 600; margin-bottom: 8px; }
.input-group input {
    width: 100%;
    padding: 12px;
    border: 1px solid #ddd;
    border-radius: 6px;
    box-sizing: border-box;
}

.form-options { text-align: right; margin-bottom: 20px; }
.forgot-link { font-size: 0.8rem; color: var(--primary); text-decoration: none; }

.btn-primary {
    width: 100%;
    padding: 12px;
    background: var(--primary);
    color: white;
    border: none;
    border-radius: 6px;
    cursor: pointer;
    font-weight: 600;
}

.divider { margin: 20px 0; color: #aaa; font-size: 0.8rem; position: relative; }

.btn-google {
    width: 100%;
    padding: 10px;
    background: white;
    border: 1px solid #ddd;
    border-radius: 6px;
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 10px;
    cursor: pointer;
    font-weight: 500;
}

.btn-google img { width: 18px; }
