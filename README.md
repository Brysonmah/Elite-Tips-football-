<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>EliteTips 2025</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        .dark-mode {
            background-color: #1a202c;
            color: #f7fafc;
        }
        .dark-mode .card {
            background-color: #2d3748;
            color: #f7fafc;
        }
        .dark-mode .nav {
            background-color: #1a202c;
            color: #f7fafc;
        }
        .dark-mode input, .dark-mode select {
            background-color: #2d3748;
            color: #f7fafc;
            border-color: #4a5568;
        }
        .paystack-button {
            transition: all 0.3s ease;
        }
        .paystack-button:hover {
            transform: translateY(-2px);
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        .prediction-card {
            transition: all 0.3s ease;
        }
        .prediction-card:hover {
            transform: translateY(-2px);
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
    </style>
</head>
<body class="bg-gray-100">
    <div id="app">
        <!-- Navigation -->
        <nav class="bg-indigo-700 text-white p-4 shadow-lg">
            <div class="container mx-auto flex justify-between items-center">
                <div class="flex items-center space-x-2">
                    <i class="fas fa-trophy text-xl"></i>
                    <h1 class="text-xl font-bold">EliteTips 2025</h1>
                </div>
                <div class="flex items-center space-x-4">
                    <button id="darkModeToggle" class="p-2 rounded-full hover:bg-indigo-600 transition">
                        <i class="fas fa-moon"></i>
                    </button>
                    <div id="authButtons">
                        <button id="loginBtn" class="px-4 py-2 bg-white text-indigo-700 rounded-lg font-medium hover:bg-gray-100 transition">
                            Login
                        </button>
                    </div>
                </div>
            </div>
        </nav>

        <!-- Main Content -->
        <main class="container mx-auto p-4">
            <!-- Home Section -->
            <section id="homeSection">
                <div class="mb-8">
                    <h2 class="text-2xl font-bold mb-4 text-gray-800 dark:text-white">Today's Top Predictions</h2>
                    <div id="predictionsList" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
                        <!-- Predictions will be loaded here -->
                    </div>
                </div>

                <div class="bg-white dark:bg-gray-800 rounded-lg shadow-lg p-6">
                    <h2 class="text-2xl font-bold mb-4 text-gray-800 dark:text-white">Premium Plans</h2>
                    <p class="text-gray-600 dark:text-gray-300 mb-6">Get access to our expert betting tips and increase your winning chances</p>
                    
                    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">
                        <div class="card bg-white dark:bg-gray-700 rounded-lg shadow-md p-6 border border-gray-200 dark:border-gray-600">
                            <h3 class="text-xl font-semibold text-gray-800 dark:text-white">Starter</h3>
                            <p class="text-gray-600 dark:text-gray-300 mt-2">KES 25</p>
                            <ul class="mt-4 space-y-2">
                                <li class="flex items-center text-gray-700 dark:text-gray-300">
                                    <i class="fas fa-check-circle text-green-500 mr-2"></i>
                                    <span>3 Games</span>
                                </li>
                                <li class="flex items-center text-gray-700 dark:text-gray-300">
                                    <i class="fas fa-check-circle text-green-500 mr-2"></i>
                                    <span>Daily Tips</span>
                                </li>
                            </ul>
                            <button class="paystack-button mt-6 w-full bg-indigo-600 hover:bg-indigo-700 text-white py-2 px-4 rounded-lg transition">
                                Subscribe Now
                            </button>
                        </div>
                        
                        <div class="card bg-white dark:bg-gray-700 rounded-lg shadow-md p-6 border border-gray-200 dark:border-gray-600">
                            <h3 class="text-xl font-semibold text-gray-800 dark:text-white">Basic</h3>
                            <p class="text-gray-600 dark:text-gray-300 mt-2">KES 50</p>
                            <ul class="mt-4 space-y-2">
                                <li class="flex items-center text-gray-700 dark:text-gray-300">
                                    <i class="fas fa-check-circle text-green-500 mr-2"></i>
                                    <span>5 Games</span>
                                </li>
                                <li class="flex items-center text-gray-700 dark:text-gray-300">
                                    <i class="fas fa-check-circle text-green-500 mr-2"></i>
                                    <span>Daily Tips</span>
                                </li>
                                <li class="flex items-center text-gray-700 dark:text-gray-300">
                                    <i class="fas fa-check-circle text-green-500 mr-2"></i>
                                    <span>HT/FT Tips</span>
                                </li>
                            </ul>
                            <button class="paystack-button mt-6 w-full bg-indigo-600 hover:bg-indigo-700 text-white py-2 px-4 rounded-lg transition">
                                Subscribe Now
                            </button>
                        </div>
                        
                        <div class="card bg-white dark:bg-gray-700 rounded-lg shadow-md p-6 border border-gray-200 dark:border-gray-600">
                            <h3 class="text-xl font-semibold text-gray-800 dark:text-white">Premium</h3>
                            <p class="text-gray-600 dark:text-gray-300 mt-2">KES 75</p>
                            <ul class="mt-4 space-y-2">
                                <li class="flex items-center text-gray-700 dark:text-gray-300">
                                    <i class="fas fa-check-circle text-green-500 mr-2"></i>
                                    <span>7 Games</span>
                                </li>
                                <li class="flex items-center text-gray-700 dark:text-gray-300">
                                    <i class="fas fa-check-circle text-green-500 mr-2"></i>
                                    <span>Daily Tips</span>
                                </li>
                                <li class="flex items-center text-gray-700 dark:text-gray-300">
                                    <i class="fas fa-check-circle text-green-500 mr-2"></i>
                                    <span>HT/FT Tips</span>
                                </li>
                                <li class="flex items-center text-gray-700 dark:text-gray-300">
                                    <i class="fas fa-check-circle text-green-500 mr-2"></i>
                                    <span>Correct Score</span>
                                </li>
                            </ul>
                            <button class="paystack-button mt-6 w-full bg-indigo-600 hover:bg-indigo-700 text-white py-2 px-4 rounded-lg transition">
                                Subscribe Now
                            </button>
                        </div>
                        
                        <div class="card bg-white dark:bg-gray-700 rounded-lg shadow-md p-6 border border-gray-200 dark:border-gray-600">
                            <h3 class="text-xl font-semibold text-gray-800 dark:text-white">VIP</h3>
                            <p class="text-gray-600 dark:text-gray-300 mt-2">KES 100</p>
                            <ul class="mt-4 space-y-2">
                                <li class="flex items-center text-gray-700 dark:text-gray-300">
                                    <i class="fas fa-check-circle text-green-500 mr-2"></i>
                                    <span>10 Games</span>
                                </li>
                                <li class="flex items-center text-gray-700 dark:text-gray-300">
                                    <i class="fas fa-check-circle text-green-500 mr-2"></i>
                                    <span>Daily Tips</span>
                                </li>
                                <li class="flex items-center text-gray-700 dark:text-gray-300">
                                    <i class="fas fa-check-circle text-green-500 mr-2"></i>
                                    <span>HT/FT Tips</span>
                                </li>
                                <li class="flex items-center text-gray-700 dark:text-gray-300">
                                    <i class="fas fa-check-circle text-green-500 mr-2"></i>
                                    <span>Correct Score</span>
                                </li>
                                <li class="flex items-center text-gray-700 dark:text-gray-300">
                                    <i class="fas fa-check-circle text-green-500 mr-2"></i>
                                    <span>24/7 Support</span>
                                </li>
                            </ul>
                            <button class="paystack-button mt-6 w-full bg-indigo-600 hover:bg-indigo-700 text-white py-2 px-4 rounded-lg transition">
                                Subscribe Now
                            </button>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Login/Signup Modal -->
            <div id="authModal" class="fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center hidden z-50">
                <div class="bg-white dark:bg-gray-800 rounded-lg shadow-xl p-6 w-full max-w-md">
                    <div class="flex justify-between items-center mb-4">
                        <h2 id="authModalTitle" class="text-2xl font-bold text-gray-800 dark:text-white">Login</h2>
                        <button id="closeAuthModal" class="text-gray-500 hover:text-gray-700 dark:text-gray-300 dark:hover:text-gray-100">
                            <i class="fas fa-times"></i>
                        </button>
                    </div>
                    
                    <form id="authForm" class="space-y-4">
                        <div>
                            <label for="email" class="block text-sm font-medium text-gray-700 dark:text-gray-300 mb-1">Email</label>
                            <input type="email" id="email" class="w-full px-3 py-2 border border-gray-300 dark:border-gray-600 rounded-md shadow-sm focus:outline-none focus:ring-indigo-500 focus:border-indigo-500 dark:bg-gray-700 dark:text-white" required>
                        </div>
                        
                        <div>
                            <label for="password" class="block text-sm font-medium text-gray-700 dark:text-gray-300 mb-1">Password</label>
                            <input type="password" id="password" class="w-full px-3 py-2 border border-gray-300 dark:border-gray-600 rounded-md shadow-sm focus:outline-none focus:ring-indigo-500 focus:border-indigo-500 dark:bg-gray-700 dark:text-white" required>
                        </div>
                        
                        <div id="confirmPasswordContainer" class="hidden">
                            <label for="confirmPassword" class="block text-sm font-medium text-gray-700 dark:text-gray-300 mb-1">Confirm Password</label>
                            <input type="password" id="confirmPassword" class="w-full px-3 py-2 border border-gray-300 dark:border-gray-600 rounded-md shadow-sm focus:outline-none focus:ring-indigo-500 focus:border-indigo-500 dark:bg-gray-700 dark:text-white">
                        </div>
                        
                        <button type="submit" id="authSubmitBtn" class="w-full flex justify-center py-2 px-4 border border-transparent rounded-md shadow-sm text-sm font-medium text-white bg-indigo-600 hover:bg-indigo-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500">
                            Login
                        </button>
                    </form>
                    
                    <div class="mt-4 text-center">
                        <button id="toggleAuthMode" class="text-sm text-indigo-600 hover:text-indigo-500 dark:text-indigo-400 dark:hover:text-indigo-300">
                            Don't have an account? Sign Up
                        </button>
                    </div>
                </div>
            </div>

            <!-- Admin Dashboard (Hidden by default) -->
            <section id="adminDashboard" class="hidden">
                <div class="bg-white dark:bg-gray-800 rounded-lg shadow-lg p-6">
                    <div class="flex justify-between items-center mb-6">
                        <h2 class="text-2xl font-bold text-gray-800 dark:text-white">Admin Dashboard</h2>
                        <button id="logoutBtn" class="px-4 py-2 bg-red-600 text-white rounded-lg hover:bg-red-700 transition">
                            Logout
                        </button>
                    </div>
                    
                    <div class="mb-6">
                        <div class="flex space-x-2">
                            <input id="newPrediction" type="text" class="flex-1 px-3 py-2 border border-gray-300 dark:border-gray-600 rounded-md shadow-sm focus:outline-none focus:ring-indigo-500 focus:border-indigo-500 dark:bg-gray-700 dark:text-white" placeholder="Enter new prediction">
                            <button id="addPredictionBtn" class="px-4 py-2 bg-green-600 text-white rounded-lg hover:bg-green-700 transition">
                                Add
                            </button>
                        </div>
                    </div>
                    
                    <div>
                        <h3 class="text-xl font-semibold text-gray-800 dark:text-white mb-4">Current Predictions</h3>
                        <div id="adminPredictionsList" class="space-y-2">
                            <!-- Admin predictions will be loaded here -->
                        </div>
                    </div>
                </div>
            </section>

            <!-- Payment Success Modal -->
            <div id="paymentSuccessModal" class="fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center hidden z-50">
                <div class="bg-white dark:bg-gray-800 rounded-lg shadow-xl p-6 w-full max-w-md text-center">
                    <div class="mb-4">
                        <i class="fas fa-check-circle text-green-500 text-5xl"></i>
                    </div>
                    <h2 class="text-2xl font-bold text-gray-800 dark:text-white mb-2">Payment Successful!</h2>
                    <p class="text-gray-600 dark:text-gray-300 mb-6">Thank you for subscribing to our service. Your predictions will be available shortly.</p>
                    <button id="closePaymentModal" class="px-4 py-2 bg-indigo-600 text-white rounded-lg hover:bg-indigo-700 transition">
                        Continue
                    </button>
                </div>
            </div>
        </main>

        <!-- Footer -->
        <footer class="bg-gray-800 text-white p-6 mt-8">
            <div class="container mx-auto">
                <div class="flex flex-col md:flex-row justify-between items-center">
                    <div class="mb-4 md:mb-0">
                        <h2 class="text-xl font-bold flex items-center">
                            <i class="fas fa-trophy mr-2"></i>
                            EliteTips 2025
                        </h2>
                        <p class="text-gray-400 mt-2">Your trusted betting tips provider</p>
                    </div>
                    
                    <div class="flex space-x-4">
                        <a href="#" class="text-gray-400 hover:text-white transition">
                            <i class="fab fa-facebook-f"></i>
                        </a>
                        <a href="#" class="text-gray-400 hover:text-white transition">
                            <i class="fab fa-twitter"></i>
                        </a>
                        <a href="#" class="text-gray-400 hover:text-white transition">
                            <i class="fab fa-instagram"></i>
                        </a>
                        <a href="#" class="text-gray-400 hover:text-white transition">
                            <i class="fab fa-telegram"></i>
                        </a>
                    </div>
                </div>
                
                <div class="border-t border-gray-700 mt-6 pt-6 text-center text-gray-400">
                    <p>&copy; 2025 EliteTips. All rights reserved.</p>
                </div>
            </div>
        </footer>
    </div>

    <script>
        // Sample data
        const predictions = [
            { id: 1, text: "Manchester United vs Liverpool - Over 2.5 Goals" },
            { id: 2, text: "Barcelona to win vs Real Madrid" },
            { id: 3, text: "PSG vs Bayern Munich - Both Teams to Score" },
            { id: 4, text: "Chelsea to win & Clean Sheet" },
            { id: 5, text: "Arsenal vs Tottenham - Draw" }
        ];

        const pricingPlans = [
            { amount: 25, games: 3 },
            { amount: 50, games: 5 },
            { amount: 75, games: 7 },
            { amount: 100, games: 10 }
        ];

        // DOM Elements
        const darkModeToggle = document.getElementById('darkModeToggle');
        const loginBtn = document.getElementById('loginBtn');
        const authModal = document.getElementById('authModal');
        const closeAuthModal = document.getElementById('closeAuthModal');
        const authModalTitle = document.getElementById('authModalTitle');
        const authForm = document.getElementById('authForm');
        const authSubmitBtn = document.getElementById('authSubmitBtn');
        const toggleAuthMode = document.getElementById('toggleAuthMode');
        const confirmPasswordContainer = document.getElementById('confirmPasswordContainer');
        const adminDashboard = document.getElementById('adminDashboard');
        const logoutBtn = document.getElementById('logoutBtn');
        const newPrediction = document.getElementById('newPrediction');
        const addPredictionBtn = document.getElementById('addPredictionBtn');
        const adminPredictionsList = document.getElementById('adminPredictionsList');
        const predictionsList = document.getElementById('predictionsList');
        const paymentSuccessModal = document.getElementById('paymentSuccessModal');
        const closePaymentModal = document.getElementById('closePaymentModal');
        const paystackButtons = document.querySelectorAll('.paystack-button');

        // State
        let isSignup = false;
        let isAdmin = false;
        let isDarkMode = false;

        // Initialize
        function init() {
            renderPredictions();
            
            // Check if admin is logged in (for demo purposes)
            const adminEmail = '12bryson96@gmail.com';
            const adminPassword = '#353612Mah';
            
            // Event Listeners
            darkModeToggle.addEventListener('click', toggleDarkMode);
            loginBtn.addEventListener('click', openAuthModal);
            closeAuthModal.addEventListener('click', closeModal);
            toggleAuthMode.addEventListener('click', toggleAuthModeHandler);
            authForm.addEventListener('submit', handleAuthSubmit);
            logoutBtn.addEventListener('click', handleLogout);
            addPredictionBtn.addEventListener('click', addPrediction);
            closePaymentModal.addEventListener('click', () => paymentSuccessModal.classList.add('hidden'));
            
            // Paystack buttons
            paystackButtons.forEach((button, index) => {
                button.addEventListener('click', (e) => {
                    e.preventDefault();
                    handlePayment(pricingPlans[index].amount, pricingPlans[index].games);
                });
            });
        }

        // Render predictions
        function renderPredictions() {
            predictionsList.innerHTML = '';
            predictions.forEach(prediction => {
                const predictionCard = document.createElement('div');
                predictionCard.className = 'prediction-card bg-white dark:bg-gray-700 rounded-lg shadow-md p-4 border border-gray-200 dark:border-gray-600';
                predictionCard.innerHTML = `
                    <div class="flex items-start">
                        <div class="flex-shrink-0 pt-1">
                            <i class="fas fa-futbol text-green-500"></i>
                        </div>
                        <div class="ml-3">
                            <p class="text-gray-800 dark:text-gray-200">${prediction.text}</p>
                            <p class="text-sm text-gray-500 dark:text-gray-400 mt-1">Posted 2 hours ago</p>
                        </div>
                    </div>
                `;
                predictionsList.appendChild(predictionCard);
            });
            
            // Render admin predictions if on admin dashboard
            if (isAdmin) {
                adminPredictionsList.innerHTML = '';
                predictions.forEach(prediction => {
                    const predictionItem = document.createElement('div');
                    predictionItem.className = 'flex justify-between items-center p-3 bg-gray-100 dark:bg-gray-700 rounded-lg';
                    predictionItem.innerHTML = `
                        <p class="text-gray-800 dark:text-gray-200">${prediction.text}</p>
                        <button class="text-red-500 hover:text-red-700 dark:hover:text-red-400" data-id="${prediction.id}">
                            <i class="fas fa-trash"></i>
                        </button>
                    `;
                    adminPredictionsList.appendChild(predictionItem);
                });
            }
        }

        // Toggle dark mode
        function toggleDarkMode() {
            isDarkMode = !isDarkMode;
            document.body.classList.toggle('dark-mode', isDarkMode);
            darkModeToggle.innerHTML = isDarkMode ? '<i class="fas fa-sun"></i>' : '<i class="fas fa-moon"></i>';
            
            // Save preference to localStorage
            localStorage.setItem('darkMode', isDarkMode);
        }

        // Auth modal handlers
        function openAuthModal() {
            authModal.classList.remove('hidden');
        }

        function closeModal() {
            authModal.classList.add('hidden');
        }

        function toggleAuthModeHandler() {
            isSignup = !isSignup;
            
            if (isSignup) {
                authModalTitle.textContent = 'Sign Up';
                authSubmitBtn.textContent = 'Sign Up';
                toggleAuthMode.textContent = 'Already have an account? Login';
                confirmPasswordContainer.classList.remove('hidden');
            } else {
                authModalTitle.textContent = 'Login';
                authSubmitBtn.textContent = 'Login';
                toggleAuthMode.textContent = "Don't have an account? Sign Up";
                confirmPasswordContainer.classList.add('hidden');
            }
        }

        function handleAuthSubmit(e) {
            e.preventDefault();
            const email = document.getElementById('email').value;
            const password = document.getElementById('password').value;
            
            // For demo purposes, check if admin credentials
            if (email === '12bryson96@gmail.com' && password === '#353612Mah') {
                isAdmin = true;
                document.getElementById('homeSection').classList.add('hidden');
                adminDashboard.classList.remove('hidden');
                closeModal();
                updateAuthUI(true);
            } else {
                // Simulate successful login for regular users
                closeModal();
                alert('Login successful!');
                updateAuthUI(true);
            }
        }

        function handleLogout() {
            isAdmin = false;
            document.getElementById('homeSection').classList.remove('hidden');
            adminDashboard.classList.add('hidden');
            updateAuthUI(false);
        }

        function updateAuthUI(isLoggedIn) {
            if (isLoggedIn) {
                if (isAdmin) {
                    authButtons.innerHTML = `
                        <button id="logoutBtn" class="px-4 py-2 bg-red-600 text-white rounded-lg hover:bg-red-700 transition">
                            Logout
                        </button>
                    `;
                    document.getElementById('logoutBtn').addEventListener('click', handleLogout);
                } else {
                    authButtons.innerHTML = `
                        <button id="logoutBtn" class="px-4 py-2 bg-red-600 text-white rounded-lg hover:bg-red-700 transition">
                            Logout
                        </button>
                    `;
                    document.getElementById('logoutBtn').addEventListener('click', handleLogout);
                }
            } else {
                authButtons.innerHTML = `
                    <button id="loginBtn" class="px-4 py-2 bg-white text-indigo-700 rounded-lg font-medium hover:bg-gray-100 transition">
                        Login
                    </button>
                `;
                document.getElementById('loginBtn').addEventListener('click', openAuthModal);
            }
        }

        function addPrediction() {
            const predictionText = newPrediction.value.trim();
            if (predictionText) {
                const newId = predictions.length + 1;
                predictions.unshift({
                    id: newId,
                    text: predictionText
                });
                newPrediction.value = '';
                renderPredictions();
            }
        }

        function handlePayment(amount, games) {
            // In a real app, this would integrate with Paystack API
            console.log(`Processing payment of KES ${amount} for ${games} games`);
            
            // Show success modal
            paymentSuccessModal.classList.remove('hidden');
        }

        // Check for saved dark mode preference
        if (localStorage.getItem('darkMode') === 'true') {
            toggleDarkMode();
        }

        // Initialize the app
        init();
    </script>
</body>
</html>
