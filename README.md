<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Canadian HVAC and Gas Services</title>
    <!-- Import Tailwind CSS from jsdelivr -->
    <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet">
    <!-- Import Font Awesome for icons -->
    <link href="https://cdn.jsdelivr.net/npm/@fortawesome/fontawesome-free@5.15.4/css/all.min.css" rel="stylesheet">
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500;600;700&family=Open+Sans:wght@400;600&display=swap" rel="stylesheet">
    
    <style>
        /* Custom CSS to supplement Tailwind */
        body {
            font-family: 'Open Sans', sans-serif;
            color: #333;
            background-color: #f9f9f9;
        }
        
        h1, h2, h3, h4, h5, h6 {
            font-family: 'Montserrat', sans-serif;
        }
        
        .hero-section {
            background: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)), url('https://cdn.jsdelivr.net/gh/genspark-project-storage/assets@main/hvac-hero.jpg');
            background-size: cover;
            background-position: center;
            background-repeat: no-repeat;
            height: 600px;
        }
        
        .service-card {
            transition: all 0.3s ease;
        }
        
        .service-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
        }
        
        .testimonial-card {
            background-color: #fff;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            padding: 20px;
            margin: 15px;
        }
        
        .footer {
            background-color: #1a202c;
            color: white;
        }
        
        .service-areas-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(150px, 1fr));
            gap: 10px;
        }
        
        .btn-primary {
            background-color: #004d99;
            color: white;
            padding: 12px 24px;
            border-radius: 4px;
            font-weight: 600;
            transition: all 0.3s ease;
        }
        
        .btn-primary:hover {
            background-color: #003366;
        }
        
        .form-input {
            width: 100%;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 4px;
            margin-bottom: 15px;
        }
        
        /* Make the entire page one continuous flow for PDF export */
        @media print {
            body {
                width: 100%;
                margin: 0;
                padding: 0;
            }
            
            .page-break {
                display: none;
            }
        }
    </style>
</head>
<body>
    <!-- Header Navigation -->
    <header class="bg-white shadow-md sticky top-0 z-50">
        <div class="container mx-auto px-4 py-3 flex justify-between items-center">
            <div class="flex items-center">
                <h1 class="text-2xl font-bold text-blue-800">Canadian HVAC & Gas</h1>
            </div>
            <div class="hidden md:flex items-center space-x-8">
                <a href="#services" class="text-gray-700 hover:text-blue-600 font-medium">Services</a>
                <a href="#about" class="text-gray-700 hover:text-blue-600 font-medium">About</a>
                <a href="#testimonials" class="text-gray-700 hover:text-blue-600 font-medium">Testimonials</a>
                <a href="#areas" class="text-gray-700 hover:text-blue-600 font-medium">Service Areas</a>
                <a href="#contact" class="text-gray-700 hover:text-blue-600 font-medium">Contact</a>
            </div>
            <div class="flex items-center">
                <div class="mr-4 text-right">
                    <p class="text-gray-600 text-sm">Call us today</p>
                    <p class="text-xl font-bold text-blue-800">(905) 555-1234</p>
                    <p class="text-sm text-gray-600">canadianhvacandgas@gmail.com</p>
                </div>
                <a href="#appointment" class="btn-primary hidden md:block">Schedule Service</a>
            </div>
            <!-- Mobile menu button -->
            <button class="md:hidden rounded-md p-2 text-gray-700 hover:text-blue-600 focus:outline-none">
                <i class="fas fa-bars text-xl"></i>
            </button>
        </div>
        <!-- Mobile menu (hidden by default) -->
        <div class="md:hidden hidden bg-white pb-4 px-4">
            <a href="#services" class="block py-2 text-gray-700 hover:text-blue-600">Services</a>
            <a href="#about" class="block py-2 text-gray-700 hover:text-blue-600">About</a>
            <a href="#testimonials" class="block py-2 text-gray-700 hover:text-blue-600">Testimonials</a>
            <a href="#areas" class="block py-2 text-gray-700 hover:text-blue-600">Service Areas</a>
            <a href="#contact" class="block py-2 text-gray-700 hover:text-blue-600">Contact</a>
            <a href="#appointment" class="btn-primary block text-center mt-4">Schedule Service</a>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero-section flex items-center justify-center">
        <div class="container mx-auto px-4 text-center text-white">
            <h1 class="text-5xl font-bold mb-6">Your Comfort is Our Priority</h1>
            <h2 class="text-3xl mb-8">Professional HVAC & Gas Services</h2>
            <p class="text-xl mb-10 max-w-3xl mx-auto">We cover all your heating, cooling, and gas needs with expert technicians and quality service.</p>
            <div class="flex flex-col sm:flex-row justify-center gap-4">
                <a href="#appointment" class="btn-primary">Schedule Service</a>
                <a href="#contact" class="bg-white text-blue-800 hover:bg-gray-100 py-3 px-6 rounded-md font-semibold">Get a Free Quote</a>
            </div>
        </div>
    </section>

    <!-- Why Choose Us Section -->
    <section id="about" class="py-20 bg-white">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-12">Why Choose Canadian HVAC and Gas?</h2>
            <p class="text-center text-xl mb-16 max-w-4xl mx-auto">With years of experience serving Oshawa and surrounding areas, we deliver reliable, high-quality service for all your HVAC and gas needs.</p>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
                <div class="text-center p-6 bg-gray-50 rounded-lg shadow-sm">
                    <div class="rounded-full bg-blue-100 w-20 h-20 flex items-center justify-center mx-auto mb-4">
                        <i class="fas fa-certificate text-blue-600 text-3xl"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Licensed Technicians</h3>
                    <p>Our team consists of fully licensed, experienced professionals.</p>
                </div>
                
                <div class="text-center p-6 bg-gray-50 rounded-lg shadow-sm">
                    <div class="rounded-full bg-blue-100 w-20 h-20 flex items-center justify-center mx-auto mb-4">
                        <i class="fas fa-phone-alt text-blue-600 text-3xl"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">24/7 Emergency Service</h3>
                    <p>We're available around the clock for any heating or cooling emergency.</p>
                </div>
                
                <div class="text-center p-6 bg-gray-50 rounded-lg shadow-sm">
                    <div class="rounded-full bg-blue-100 w-20 h-20 flex items-center justify-center mx-auto mb-4">
                        <i class="fas fa-dollar-sign text-blue-600 text-3xl"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Competitive Pricing</h3>
                    <p>Fair and transparent pricing with no hidden fees or surprises.</p>
                </div>
                
                <div class="text-center p-6 bg-gray-50 rounded-lg shadow-sm">
                    <div class="rounded-full bg-blue-100 w-20 h-20 flex items-center justify-center mx-auto mb-4">
                        <i class="fas fa-check-circle text-blue-600 text-3xl"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Satisfaction Guaranteed</h3>
                    <p>We stand behind our work with a 100% satisfaction guarantee.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" class="py-20 bg-gray-100">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-12">Our Services</h2>
            <p class="text-center text-xl mb-16 max-w-4xl mx-auto">Explore our comprehensive range of HVAC and gas services designed to keep your home comfortable all year round.</p>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-10">
                <div class="service-card bg-white rounded-lg overflow-hidden shadow-md">
                    <div class="h-48 bg-blue-600 flex items-center justify-center">
                        <i class="fas fa-fire text-white text-6xl"></i>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-3">Heating Services</h3>
                        <p class="mb-4">We offer comprehensive heating services including installation, repair, and maintenance for furnaces, boilers, and heat pumps.</p>
                        <ul class="mb-4 space-y-2">
                            <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Furnace Installation & Repair</li>
                            <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Boiler Services</li>
                            <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Heat Pump Maintenance</li>
                            <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Emergency Heating Repairs</li>
                        </ul>
                        <a href="#contact" class="text-blue-600 font-bold hover:underline">Learn More →</a>
                    </div>
                </div>
                
                <div class="service-card bg-white rounded-lg overflow-hidden shadow-md">
                    <div class="h-48 bg-blue-600 flex items-center justify-center">
                        <i class="fas fa-snowflake text-white text-6xl"></i>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-3">Cooling Services</h3>
                        <p class="mb-4">Keep your home cool and comfortable with our expert air conditioning installation, repair, and maintenance services.</p>
                        <ul class="mb-4 space-y-2">
                            <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> AC Installation & Replacement</li>
                            <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> AC Repair & Maintenance</li>
                            <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Ductless Mini-Split Systems</li>
                            <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Commercial Cooling Solutions</li>
                        </ul>
                        <a href="#contact" class="text-blue-600 font-bold hover:underline">Learn More →</a>
                    </div>
                </div>
                
                <div class="service-card bg-white rounded-lg overflow-hidden shadow-md">
                    <div class="h-48 bg-blue-600 flex items-center justify-center">
                        <i class="fas fa-burn text-white text-6xl"></i>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-3">Gas Services</h3>
                        <p class="mb-4">Our licensed gas technicians provide safe and reliable gas fitting, installation, and repair services for your home.</p>
                        <ul class="mb-4 space-y-2">
                            <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Gas Line Installation</li>
                            <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Gas Leak Detection & Repair</li>
                            <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Gas Appliance Installation</li>
                            <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Gas Fireplace Services</li>
                        </ul>
                        <a href="#contact" class="text-blue-600 font-bold hover:underline">Learn More →</a>
                    </div>
                </div>
                
                <div class="service-card bg-white rounded-lg overflow-hidden shadow-md">
                    <div class="h-48 bg-blue-600 flex items-center justify-center">
                        <i class="fas fa-tools text-white text-6xl"></i>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-3">Maintenance & Tune-ups</h3>
                        <p class="mb-4">Regular maintenance keeps your HVAC systems running efficiently and prevents costly breakdowns.</p>
                        <ul class="mb-4 space-y-2">
                            <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Seasonal Maintenance Plans</li>
                            <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Furnace Tune-ups</li>
                            <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> AC System Inspections</li>
                            <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Filter Replacement</li>
                        </ul>
                        <a href="#contact" class="text-blue-600 font-bold hover:underline">Learn More →</a>
                    </div>
                </div>
                
                <div class="service-card bg-white rounded-lg overflow-hidden shadow-md">
                    <div class="h-48 bg-blue-600 flex items-center justify-center">
                        <i class="fas fa-home text-white text-6xl"></i>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-3">Indoor Air Quality</h3>
                        <p class="mb-4">Improve the air quality in your home with our professional air purification and ventilation services.</p>
                        <ul class="mb-4 space-y-2">
                            <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Air Purifier Installation</li>
                            <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Humidifier & Dehumidifier Services</li>
                            <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Duct Cleaning & Sealing</li>
                            <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Ventilation System Maintenance</li>
                        </ul>
                        <a href="#contact" class="text-blue-600 font-bold hover:underline">Learn More →</a>
                    </div>
                </div>
                
                <div class="service-card bg-white rounded-lg overflow-hidden shadow-md">
                    <div class="h-48 bg-blue-600 flex items-center justify-center">
                        <i class="fas fa-building text-white text-6xl"></i>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-3">Commercial HVAC</h3>
                        <p class="mb-4">Specialized HVAC solutions designed for businesses, commercial buildings, and industrial facilities.</p>
                        <ul class="mb-4 space-y-2">
                            <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Commercial HVAC Installation</li>
                            <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Preventative Maintenance Programs</li>
                            <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> System Upgrades & Retrofits</li>
                            <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Energy Efficiency Solutions</li>
                        </ul>
                        <a href="#contact" class="text-blue-600 font-bold hover:underline">Learn More →</a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials Section -->
    <section id="testimonials" class="py-20 bg-white">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-12">What Our Customers Say</h2>
            <p class="text-center text-xl mb-16 max-w-4xl mx-auto">Hear from our satisfied customers about their experience with Canadian HVAC and Gas.</p>
            
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                <div class="testimonial-card">
                    <div class="flex items-center mb-4">
                        <div class="text-yellow-400 flex mr-2">
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                        </div>
                        <span class="text-gray-600">5.0</span>
                    </div>
                    <p class="italic mb-4">"Our furnace stopped working during the coldest night of the year. Canadian HVAC and Gas responded to our emergency call within an hour and had our heat back on before bedtime. Excellent service!"</p>
                    <div class="flex items-center">
                        <div class="mr-3">
                            <div class="w-12 h-12 rounded-full bg-gray-300 flex items-center justify-center">
                                <i class="fas fa-user text-gray-600"></i>
                            </div>
                        </div>
                        <div>
                            <h4 class="font-semibold">Michael Thompson</h4>
                            <p class="text-sm text-gray-600">Oshawa, ON</p>
                        </div>
                    </div>
                </div>
                
                <div class="testimonial-card">
                    <div class="flex items-center mb-4">
                        <div class="text-yellow-400 flex mr-2">
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                        </div>
                        <span class="text-gray-600">5.0</span>
                    </div>
                    <p class="italic mb-4">"I've been using Canadian HVAC and Gas for over 5 years now for all my heating and cooling needs. Their technicians are always professional, on time, and take the time to explain everything."</p>
                    <div class="flex items-center">
                        <div class="mr-3">
                            <div class="w-12 h-12 rounded-full bg-gray-300 flex items-center justify-center">
                                <i class="fas fa-user text-gray-600"></i>
                            </div>
                        </div>
                        <div>
                            <h4 class="font-semibold">Sarah Johnson</h4>
                            <p class="text-sm text-gray-600">Whitby, ON</p>
                        </div>
                    </div>
                </div>
                
                <div class="testimonial-card">
                    <div class="flex items-center mb-4">
                        <div class="text-yellow-400 flex mr-2">
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                        </div>
                        <span class="text-gray-600">5.0</span>
                    </div>
                    <p class="italic mb-4">"The team at Canadian HVAC and Gas installed our new high-efficiency furnace and air conditioner. The installation was smooth, and they left our home spotless. Our energy bills have decreased significantly!"</p>
                    <div class="flex items-center">
                        <div class="mr-3">
                            <div class="w-12 h-12 rounded-full bg-gray-300 flex items-center justify-center">
                                <i class="fas fa-user text-gray-600"></i>
                            </div>
                        </div>
                        <div>
                            <h4 class="font-semibold">David Wilson</h4>
                            <p class="text-sm text-gray-600">Ajax, ON</p>
                        </div>
                    </div>
                </div>
                
                <div class="testimonial-card">
                    <div class="flex items-center mb-4">
                        <div class="text-yellow-400 flex mr-2">
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                        </div>
                        <span class="text-gray-600">5.0</span>
                    </div>
                    <p class="italic mb-4">"I called about a suspected gas leak and they were at my door within 30 minutes. The technician was thorough, professional, and fixed the issue quickly. Great peace of mind knowing they're just a call away."</p>
                    <div class="flex items-center">
                        <div class="mr-3">
                            <div class="w-12 h-12 rounded-full bg-gray-300 flex items-center justify-center">
                                <i class="fas fa-user text-gray-600"></i>
                            </div>
                        </div>
                        <div>
                            <h4 class="font-semibold">Jennifer Lee</h4>
                            <p class="text-sm text-gray-600">Pickering, ON</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Service Areas Section -->
    <section id="areas" class="py-20 bg-gray-100">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-12">Our Service Areas</h2>
            <p class="text-center text-xl mb-16 max-w-4xl mx-auto">We proudly serve Oshawa and surrounding areas, including Whitby, Ajax, Pickering, Scarborough, Bowmanville, Newcastle, Newmarket, Port Perry, and Lindsay.</p>
            
            <div class="service-areas-grid max-w-5xl mx-auto">
                <div class="bg-white p-4 text-center rounded-lg shadow-sm">
                    <i class="fas fa-map-marker-alt text-blue-600 mb-2"></i>
                    <h3 class="font-semibold">Oshawa</h3>
                </div>
                <div class="bg-white p-4 text-center rounded-lg shadow-sm">
                    <i class="fas fa-map-marker-alt text-blue-600 mb-2"></i>
                    <h3 class="font-semibold">Whitby</h3>
                </div>
                <div class="bg-white p-4 text-center rounded-lg shadow-sm">
                    <i class="fas fa-map-marker-alt text-blue-600 mb-2"></i>
                    <h3 class="font-semibold">Ajax</h3>
                </div>
                <div class="bg-white p-4 text-center rounded-lg shadow-sm">
                    <i class="fas fa-map-marker-alt text-blue-600 mb-2"></i>
                    <h3 class="font-semibold">Pickering</h3>
                </div>
                <div class="bg-white p-4 text-center rounded-lg shadow-sm">
                    <i class="fas fa-map-marker-alt text-blue-600 mb-2"></i>
                    <h3 class="font-semibold">Scarborough</h3>
                </div>
                <div class="bg-white p-4 text-center rounded-lg shadow-sm">
                    <i class="fas fa-map-marker-alt text-blue-600 mb-2"></i>
                    <h3 class="font-semibold">Bowmanville</h3>
                </div>
                <div class="bg-white p-4 text-center rounded-lg shadow-sm">
                    <i class="fas fa-map-marker-alt text-blue-600 mb-2"></i>
                    <h3 class="font-semibold">Newcastle</h3>
                </div>
                <div class="bg-white p-4 text-center rounded-lg shadow-sm">
                    <i class="fas fa-map-marker-alt text-blue-600 mb-2"></i>
                    <h3 class="font-semibold">Newmarket</h3>
                </div>
                <div class="bg-white p-4 text-center rounded-lg shadow-sm">
                    <i class="fas fa-map-marker-alt text-blue-600 mb-2"></i>
                    <h3 class="font-semibold">Port Perry</h3>
                </div>
                <div class="bg-white p-4 text-center rounded-lg shadow-sm">
                    <i class="fas fa-map-marker-alt text-blue-600 mb-2"></i>
                    <h3 class="font-semibold">Lindsay</h3>
                </div>
            </div>
        </div>
    </section>

    <!-- Appointment & Contact Section -->
    <section id="appointment" class="py-20 bg-white">
        <div class="container mx-auto px-4">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-16">
                <!-- Appointment Form -->
                <div>
                    <h2 class="text-3xl font-bold mb-8">Schedule Your Appointment</h2>
                    <p class="mb-6">Book your service appointment today. Our team will get back to you promptly to confirm your booking.</p>
                    
                    <!-- Form using FormSubmit.co that sends to both emails -->
                    <form id="appointmentForm" action="https://formsubmit.co/jamiesonmills@live.com" method="POST" class="space-y-4">
                        <!-- Hidden input for the second email -->
                        <input type="hidden" name="_next" value="https://yourwebsite.com/thank-you">
                        <input type="hidden" name="_cc" value="canadianhvacandgas@gmail.com">
                        <input type="hidden" name="_subject" value="New Appointment Request">
                        <input type="hidden" name="_template" value="table">
                        
                        <div>
                            <label for="name" class="block mb-2 font-medium">Full Name</label>
                            <input type="text" id="name" name="name" class="form-input" required>
                        </div>
                        
                        <div>
                            <label for="email" class="block mb-2 font-medium">Email Address</label>
                            <input type="email" id="email" name="email" class="form-input" required>
                        </div>
                        
                        <div>
                            <label for="phone" class="block mb-2 font-medium">Phone Number</label>
                            <input type="tel" id="phone" name="phone" class="form-input" required>
                        </div>
                        
                        <div>
                            <label for="service" class="block mb-2 font-medium">Service Needed</label>
                            <select id="service" name="service" class="form-input" required>
                                <option value="">Select a service</option>
                                <option value="Heating">Heating Service</option>
                                <option value="Cooling">Cooling Service</option>
                                <option value="Gas">Gas Service</option>
                                <option value="Maintenance">Maintenance</option>
                                <option value="Air Quality">Indoor Air Quality</option>
                                <option value="Commercial">Commercial HVAC</option>
                            </select>
                        </div>
                        
                        <div>
                            <label for="date" class="block mb-2 font-medium">Preferred Date</label>
                            <input type="date" id="date" name="date" class="form-input" required>
                        </div>
                        
                        <div>
                            <label for="time" class="block mb-2 font-medium">Preferred Time</label>
                            <select id="time" name="time" class="form-input" required>
                                <option value="">Select a time</option>
                                <option value="Morning">Morning (8am - 12pm)</option>
                                <option value="Afternoon">Afternoon (12pm - 4pm)</option>
                                <option value="Evening">Evening (4pm - 8pm)</option>
                            </select>
                        </div>
                        
                        <div>
                            <label for="message" class="block mb-2 font-medium">Additional Information</label>
                            <textarea id="message" name="message" rows="4" class="form-input"></textarea>
                        </div>
                        
                        <div>
                            <button type="submit" class="btn-primary w-full">Schedule Appointment</button>
                        </div>
                    </form>
                </div>
                
                <!-- Contact Information -->
                <div id="contact">
                    <h2 class="text-3xl font-bold mb-8">Contact Us</h2>
                    <p class="mb-10">Have questions or need immediate assistance? Reach out to our friendly team today.</p>
                    
                    <div class="space-y-8">
                        <div class="flex items-start">
                            <div class="bg-blue-100 rounded-full p-3 mr-4">
                                <i class="fas fa-phone text-blue-600"></i>
                            </div>
                            <div>
                                <h3 class="font-bold text-lg">Phone</h3>
                                <p class="text-xl">(905) 555-1234</p>
                                <p class="text-gray-600">Available 24/7 for emergencies</p>
                            </div>
                        </div>
                        
                        <div class="flex items-start">
                            <div class="bg-blue-100 rounded-full p-3 mr-4">
                                <i class="fas fa-envelope text-blue-600"></i>
                            </div>
                            <div>
                                <h3 class="font-bold text-lg">Email</h3>
                                <p class="text-xl">canadianhvacandgas@gmail.com</p>
                                <p class="text-gray-600">We'll respond within 24 hours</p>
                            </div>
                        </div>
                        
                        <div class="flex items-start">
                            <div class="bg-blue-100 rounded-full p-3 mr-4">
                                <i class="fas fa-clock text-blue-600"></i>
                            </div>
                            <div>
                                <h3 class="font-bold text-lg">Hours</h3>
                                <p>Monday - Friday: 8am - 8pm</p>
                                <p>Saturday: 9am - 5pm</p>
                                <p>Sunday: 10am - 4pm</p>
                                <p class="text-blue-600 font-semibold mt-1">24/7 Emergency Service Available</p>
                            </div>
                        </div>
                        
                        <div class="flex items-start">
                            <div class="bg-blue-100 rounded-full p-3 mr-4">
                                <i class="fas fa-map-marker-alt text-blue-600"></i>
                            </div>
                            <div>
                                <h3 class="font-bold text-lg">Office Location</h3>
                                <p>Oshawa, Ontario</p>
                                <p class="text-gray-600">With technicians in Kawartha Lakes, Ajax, and surrounding areas</p>
                            </div>
                        </div>
                    </div>
                    
                    <!-- Get a Free Quote Form -->
                    <div class="mt-12">
                        <h3 class="text-2xl font-bold mb-6">Get a Free Quote</h3>
                        <form id="quoteForm" action="https://formsubmit.co/jamiesonmills@live.com" method="POST" class="space-y-4">
                            <input type="hidden" name="_next" value="https://yourwebsite.com/thank-you">
                            <input type="hidden" name="_cc" value="canadianhvacandgas@gmail.com">
                            <input type="hidden" name="_subject" value="New Quote Request">
                            <input type="hidden" name="_template" value="table">
                            
                            <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                                <div>
                                    <input type="text" name="name" placeholder="Your Name" class="form-input" required>
                                </div>
                                <div>
                                    <input type="email" name="email" placeholder="Email Address" class="form-input" required>
                                </div>
                            </div>
                            
                            <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                                <div>
                                    <input type="tel" name="phone" placeholder="Phone Number" class="form-input" required>
                                </div>
                                <div>
                                    <select name="service" class="form-input" required>
                                        <option value="">Select Service</option>
                                        <option value="Heating">Heating</option>
                                        <option value="Cooling">Cooling</option>
                                        <option value="Gas">Gas Services</option>
                                        <option value="Other">Other</option>
                                    </select>
                                </div>
                            </div>
                            
                            <div>
                                <textarea name="message" placeholder="Tell us about your project or requirements" rows="3" class="form-input" required></textarea>
                            </div>
                            
                            <div>
                                <button type="submit" class="btn-primary w-full">Get Free Quote</button>
                            </div>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="footer py-12">
        <div class="container mx-auto px-4">
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
                <div>
                    <h3 class="text-xl font-bold text-white mb-4">Canadian HVAC & Gas</h3>
                    <p class="text-gray-300 mb-4">Your trusted HVAC and gas service provider in Oshawa and surrounding areas. Licensed, insured, and ready to serve you.</p>
                    <div class="flex space-x-4">
                        <a href="#" class="text-white hover:text-blue-300"><i class="fab fa-facebook-f"></i></a>
                        <a href="#" class="text-white hover:text-blue-300"><i class="fab fa-twitter"></i></a>
                        <a href="#" class="text-white hover:text-blue-300"><i class="fab fa-instagram"></i></a>
                        <a href="#" class="text-white hover:text-blue-300"><i class="fab fa-linkedin-in"></i></a>
                    </div>
                </div>
                
                <div>
                    <h3 class="text-xl font-bold text-white mb-4">Quick Links</h3>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-300 hover:text-white">Home</a></li>
                        <li><a href="#services" class="text-gray-300 hover:text-white">Services</a></li>
                        <li><a href="#about" class="text-gray-300 hover:text-white">About Us</a></li>
                        <li><a href="#testimonials" class="text-gray-300 hover:text-white">Testimonials</a></li>
                        <li><a href="#areas" class="text-gray-300 hover:text-white">Service Areas</a></li>
                        <li><a href="#contact" class="text-gray-300 hover:text-white">Contact Us</a></li>
                    </ul>
                </div>
                
                <div>
                    <h3 class="text-xl font-bold text-white mb-4">Services</h3>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-300 hover:text-white">Heating Services</a></li>
                        <li><a href="#" class="text-gray-300 hover:text-white">Cooling Services</a></li>
                        <li><a href="#" class="text-gray-300 hover:text-white">Gas Services</a></li>
                        <li><a href="#" class="text-gray-300 hover:text-white">Maintenance & Tune-ups</a></li>
                        <li><a href="#" class="text-gray-300 hover:text-white">Indoor Air Quality</a></li>
                        <li><a href="#" class="text-gray-300 hover:text-white">Commercial HVAC</a></li>
                    </ul>
                </div>
                
                <div>
                    <h3 class="text-xl font-bold text-white mb-4">Contact</h3>
                    <ul class="space-y-2">
                        <li class="flex items-start">
                            <i class="fas fa-phone text-blue-400 mt-1 mr-3"></i>
                            <span class="text-gray-300">(905) 555-1234</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-envelope text-blue-400 mt-1 mr-3"></i>
                            <span class="text-gray-300">canadianhvacandgas@gmail.com</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-map-marker-alt text-blue-400 mt-1 mr-3"></i>
                            <span class="text-gray-300">Oshawa, Ontario</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-clock text-blue-400 mt-1 mr-3"></i>
                            <span class="text-gray-300">24/7 Emergency Service</span>
                        </li>
                    </ul>
                </div>
            </div>
            
            <div class="border-t border-gray-700 mt-12 pt-8 text-center">
                <p class="text-gray-400">&copy; 2023 Canadian HVAC & Gas. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <!-- JavaScript -->
    <script>
        // Mobile menu toggle
        document.addEventListener('DOMContentLoaded', function() {
            const menuButton = document.querySelector('.md\\:hidden.rounded-md.p-2');
            const mobileMenu = document.querySelector('.md\\:hidden.hidden.bg-white');
            
            if (menuButton && mobileMenu) {
                menuButton.addEventListener('click', function() {
                    mobileMenu.classList.toggle('hidden');
                });
            }
            
            // Function to save user information to "user list" file
            function saveUserInfo(formData) {
                // In a real implementation, this would send data to a server to save to a file
                // For this demo, we'll use localStorage to simulate saving data
                const existingData = localStorage.getItem('userList') ? JSON.parse(localStorage.getItem('userList')) : [];
                existingData.push(formData);
                localStorage.setItem('userList', JSON.stringify(existingData));
                
                console.log('User information saved to "user list"');
                console.log(formData);
            }
            
            // Handle appointment form submission
            const appointmentForm = document.getElementById('appointmentForm');
            if (appointmentForm) {
                appointmentForm.addEventListener('submit', function(e) {
                    // Don't prevent default as we want the form to submit to FormSubmit.co
                    
                    // Get form data to save locally
                    const formData = {
                        type: 'appointment',
                        name: document.getElementById('name').value,
                        email: document.getElementById('email').value,
                        phone: document.getElementById('phone').value,
                        service: document.getElementById('service').value,
                        date: document.getElementById('date').value,
                        time: document.getElementById('time').value,
                        message: document.getElementById('message').value,
                        submittedAt: new Date().toISOString()
                    };
                    
                    // Save user information
                    saveUserInfo(formData);
                });
            }
            
            // Handle quote form submission
            const quoteForm = document.getElementById('quoteForm');
            if (quoteForm) {
                quoteForm.addEventListener('submit', function(e) {
                    // Don't prevent default as we want the form to submit to FormSubmit.co
                    
                    // Get form data to save locally
                    const formData = {
                        type: 'quote',
                        name: this.querySelector('[name="name"]').value,
                        email: this.querySelector('[name="email"]').value,
                        phone: this.querySelector('[name="phone"]').value,
                        service: this.querySelector('[name="service"]').value,
                        message: this.querySelector('[name="message"]').value,
                        submittedAt: new Date().toISOString()
                    };
                    
                    // Save user information
                    saveUserInfo(formData);
                });
            }
        });
    </script>

    <!-- GitHub Deployment Instructions (Hidden in production) -->
    <!-- 
    GitHub Deployment Instructions:
    
    1. Create a new GitHub repository
    2. Clone the repository to your local machine
    3. Add the following files to the repository:
       - index.html (this file)
       - Create a css folder with styles.css (if you split the CSS)
       - Create a js folder with scripts.js (if you split the JavaScript)
       - Add any image assets needed
    4. Commit and push the files to GitHub
    5. Enable GitHub Pages:
       - Go to your repository settings
       - Scroll down to the GitHub Pages section
       - Select the main branch as the source
       - Click Save
    6. Your website will be published at https://yourusername.github.io/repositoryname/
    
    Form Setup:
    1. The forms are set up using FormSubmit.co to send to both jamiesonmills@live.com and canadianhvacandgas@gmail.com
    2. You may need to confirm your email with FormSubmit.co when the first form is submitted
    3. The forms save user information using JavaScript to localStorage (in a real deployment, you would use server-side code)
    
    Custom Domain Setup (Optional):
    1. Purchase a domain name from a registrar
    2. In your GitHub repository settings, add the custom domain
    3. Configure your domain's DNS settings to point to GitHub Pages
    -->
</body>
</html>
