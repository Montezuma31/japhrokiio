<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Street Food Menu</title>
    <!-- Load Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Load Handwritten Fonts (Gochi Hand and Permanent Marker) -->
    <link href="https://fonts.googleapis.com/css2?family=Gochi+Hand&family=Permanent+Marker&family=Inter:wght@400;700;900&display=swap" rel="stylesheet">
    <style>
        /* Define Font Classes */
        .body-font {
            font-family: 'Inter', sans-serif;
        }
        .header-font {
            font-family: 'Gochi Hand', cursive; /* Handwritten, energetic title font */
        }
        .item-font {
            font-family: 'Permanent Marker', cursive; /* Bold, marker-style handwritten font for items and prices */
        }
        
        /* Street Food Palette */
        .street-bg {
            background-color: #380D0B; /* Dark, warm background */
            background-image: repeating-linear-gradient(45deg, #4d1d1b 0, #4d1d1b 10px, #380d0b 10px, #380d0b 20px);
        }
        .menu-card {
            background-color: #FDFDFA; /* Paper/Whiteboard base */
            border: 8px solid #FFC300; /* Bright Yellow border */
            border-style: double;
            box-shadow: 10px 10px 0 #D63447; /* Offset Red Shadow */
        }
        .street-red {
            color: #D63447; /* Strong Red */
        }
        .street-yellow {
            color: #FFC300; /* Bright Yellow */
        }
        
        /* Stylized Header Look */
        .header-box {
            background-color: #D63447;
            border-bottom: 5px solid #000;
            text-shadow: 2px 2px 0 #FFC300;
        }
        
        /* Item Divider Style */
        .item-divider {
            border: 2px solid #D63447;
            border-style: dotted;
            margin: 0.5rem 0;
        }

        /* Price Tag */
        .price-tag {
            background-color: #FFC300;
            color: #D63447;
            border: 3px solid #000;
            padding: 0.5rem 1rem;
            transform: rotate(-3deg); /* Give it a playful tilt */
            white-space: nowrap; /* Prevent price from wrapping */
        }
        
        /* Ensure item names and prices use the handwritten font */
        .menu-card .item-font {
            font-family: 'Permanent Marker', cursive;
        }
    </style>
</head>
<body class="min-h-screen p-4 sm:p-8 flex items-center justify-center street-bg body-font text-gray-900">

    <!-- The Menu Card - Indian Street Food Aesthetic -->
    <div class="w-full max-w-2xl menu-card rounded-xl overflow-hidden relative">
        
        <!-- Header Section -->
        <header class="header-box p-4 sm:p-6 text-center">
            <p class="text-xl text-black font-extrabold uppercase tracking-widest leading-none">
                CIRCUS MAXIMUS PRESENTS
            </p>
            <h2 class="text-5xl sm:text-7xl header-font text-white mt-2 leading-none tracking-tight">
                THE FADDU MENU
            </h2>
            <div class="h-2 w-16 bg-white mx-auto mt-3 rounded-full"></div>
        </header>

        <!-- Main Items Section -->
        <main class="p-6 sm:p-8">
            <h3 class="text-3xl font-extrabold text-black pb-2 item-font uppercase leading-tight tracking-wider border-b-4 border-black">
                ITEM BOMB
            </h3>
            
            <div class="space-y-4 pt-4">
                
                <!-- Item 1: Bhalla-e-Azam -->
                <div class="flex justify-between items-start bg-yellow-50 p-3 rounded-lg border-2 border-red-500">
                    <div class="flex flex-col">
                        <span class="text-3xl font-bold street-red item-font uppercase">Bhalla-e-Azam</span>
                        <span class="text-sm text-gray-700 font-semibold body-font">The Emperor's Snack — King of all Bhallas!</span>
                    </div>
                    <span class="text-3xl font-black price-tag item-font">50 ₹</span>
                </div>
                <div class="item-divider"></div>

                <!-- Item 2: Tagda-Ragda Samosa -->
                <div class="flex justify-between items-center py-2 px-1">
                    <div class="flex flex-col">
                        <span class="text-2xl font-bold text-black item-font uppercase">Tagda-Ragda Samosa</span>
                        <span class="text-sm text-gray-600 body-font">The robust, powerful samosa mash-up.</span>
                    </div>
                    <span class="text-3xl font-bold street-red item-font">30 ₹</span>
                </div>
                <div class="item-divider"></div>


                <!-- Item 3: Chip-Mix -->
                <div class="flex justify-between items-center py-2 px-1">
                    <div class="flex flex-col">
                        <span class="text-2xl font-bold text-black item-font uppercase">Chip-Mix</span>
                        <span class="text-sm text-gray-600 body-font">Crisp, zesty, and chaat-ified chips.</span>
                    </div>
                    <span class="text-3xl font-bold street-red item-font">30 ₹</span>
                </div>
                <div class="item-divider"></div>

                <!-- Item 4: Oreo Mousse -->
                <div class="flex justify-between items-center py-2 px-1">
                    <div class="flex flex-col">
                        <span class="text-2xl font-bold text-black item-font uppercase">Oreo Mousse</span>
                        <span class="text-sm text-gray-600 body-font">Sweet, creamy, and decadent treat.</span>
                    </div>
                    <span class="text-3xl font-bold street-red item-font">30 ₹</span>
                </div>
                <div class="item-divider"></div>

                <!-- Item 5: Thanda-e-Maza -->
                <div class="flex justify-between items-center py-2 px-1">
                    <div class="flex flex-col">
                        <span class="text-2xl font-bold text-black item-font uppercase">Thanda-e-Maza</span>
                        <span class="text-sm text-gray-600 body-font">The ultimate cooler, full of Maza.</span>
                    </div>
                    <span class="text-3xl font-bold street-red item-font">20 ₹</span>
                </div>

                <!-- Divider between sections -->
                <div class="h-2 bg-black w-full my-6"></div>

                <!-- Meal Section -->
                <h3 class="text-3xl font-extrabold text-black pb-2 item-font uppercase leading-tight tracking-wider border-b-4 border-black">
                    MEAL DEAL
                </h3>
                
                <!-- Highlighted Meal Box - uses bright yellow to stand out -->
                <div class="bg-street-yellow p-5 rounded-lg border-4 border-black relative transform rotate-1">
                    <div class="flex justify-between items-start pb-2">
                        <div class="flex flex-col">
                            <span class="text-4xl sm:text-5xl header-font text-street-red tracking-tight uppercase" style="text-shadow: 2px 2px 0 #000;">
                                Doonite Meal
                            </span>
                            <span class="text-base font-medium text-black mt-1 font-extrabold body-font">
                                CHIP-MIX + OREO MOUSSE + THANDA-E-MAZA
                            </span>
                        </div>
                        <span class="text-4xl sm:text-5xl font-black street-red item-font">60 ₹</span>
                    </div>
                    <p class="text-lg font-bold text-black text-center pt-2 mt-4 border-t-2 border-dashed border-black item-font">
                        HUGE SAVINGS! Get all 3 items for a steal!
                    </p>
                </div>
            </div>
            
        </main>
    </div>

</body>
</html>
