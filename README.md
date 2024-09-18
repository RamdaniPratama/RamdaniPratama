<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PPOB Application</title>
    <link href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <nav class="navbar navbar-expand-lg navbar-dark bg-primary">
        <a class="navbar-brand" href="#">PPOB App</a>
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav">
                <li class="nav-item active">
                    <a class="nav-link" href="#">Home <span class="sr-only">(current)</span></a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#services">Services</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#transactions">Transactions</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#profile">Profile</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#contact">Contact</a>
                </li>
            </ul>
        </div>
    </nav>

    <header class="bg-primary text-white text-center py-5">
        <div class="container">
            <h1 class="display-4">Top Up Your Services</h1>
            <p class="lead">Pulsa, Kuota, e-Wallet, and more</p>
        </div>
    </header>

    <section id="services" class="my-5">
        <div class="container">
            <h2 class="text-center mb-4">Available Services</h2>
            <div class="row">
                <div class="col-md-8 mx-auto">
                    <form id="payment-form">
                        <div class="form-group">
                            <label for="service">Select Service</label>
                            <select id="service" class="form-control">
                                <option value="pulsa">Pulsa</option>
                                <option value="kuota">Kuota</option>
                                <option value="ewallet">e-Wallet</option>
                                <option value="payment">Other Payment</option>
                            </select>
                        </div>
                        <div class="form-group">
                            <label for="amount">Amount</label>
                            <input type="number" id="amount" class="form-control" placeholder="Enter amount" required>
                        </div>
                        <button type="submit" class="btn btn-primary btn-lg">Submit</button>
                    </form>
                    <div id="result" class="mt-4"></div>
                </div>
            </div>
        </div>
    </section>

    <section id="transactions" class="my-5 bg-light py-5">
        <div class="container">
            <h2 class="text-center mb-4">Transaction History</h2>
            <div class="table-responsive">
                <table class="table table-striped">
                    <thead>
                        <tr>
                            <th>#</th>
                            <th>Service</th>
                            <th>Amount</th>
                            <th>Date</th>
                        </tr>
                    </thead>
                    <tbody id="transaction-list">
                        <!-- Transactions will be dynamically inserted here -->
                    </tbody>
                </table>
            </div>
        </div>
    </section>

    <section id="profile" class="my-5">
        <div class="container">
            <h2 class="text-center mb-4">User Profile</h2>
            <div class="row">
                <div class="col-md-6 mx-auto">
                    <form id="profile-form">
                        <div class="form-group">
                            <label for="username">Username</label>
                            <input type="text" id="username" class="form-control" placeholder="Enter your username" required>
                        </div>
                        <div class="form-group">
                            <label for="email">Email</label>
                            <input type="email" id="email" class="form-control" placeholder="Enter your email" required>
                        </div>
                        <div class="form-group">
                            <label for="phone">Phone</label>
                            <input type="text" id="phone" class="form-control" placeholder="Enter your phone number" required>
                        </div>
                        <button type="submit" class="btn btn-primary btn-lg">Update Profile</button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <section id="contact" class="my-5 bg-light py-5">
        <div class="container">
            <h2 class="text-center mb-4">Contact Us</h2>
            <p class="text-center">If you have any questions or need assistance, please reach out to us.</p>
            <div class="text-center">
                <a href="https://wa.me/081286396082?text=Hello%2C%20I%20would%20like%20to%20get%20in%20touch%20with%20you" class="btn btn-success btn-lg" target="_blank">Contact via WhatsApp</a>
            </div>
        </div>
    </section>

    <footer class="bg-dark text-white text-center py-4">
        <div class="container">
            <p>&copy; 2024 PPOB Application. All rights reserved.</p>
        </div>
    </footer>

    <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.11.6/dist/umd/popper.min.js"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
    <script src="scripts.js"></script>
</body>
</html>
