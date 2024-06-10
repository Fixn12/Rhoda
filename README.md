
 <!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Digital Card for Crush</title>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/tailwindcss/2.2.19/tailwind.min.css" rel="stylesheet">
    <style>
        .fade-in {
            animation: fadeIn ease 3s;
        }

        @keyframes fadeIn {
            0% {
                opacity: 0;
            }

            100% {
                opacity: 1;
            }
        }

        .hidden-message {
            display: none;
        }

        .visible-message {
            display: block;
            animation: slideIn ease 1s;
        }

        @keyframes slideIn {
            0% {
                transform: translateY(20px);
                opacity: 0;
            }

            100% {
                transform: translateY(0);
                opacity: 1;
            }
        }
    </style>
</head>

<body class="bg-blue-100 flex items-center justify-center min-h-screen">
    <div class="bg-white p-8 rounded-lg shadow-lg max-w-sm fade-in">
        <div class="text-center mb-4">
            <img src="aww.jpg" alt="Profile Picture" class="rounded-full w-32 mx-auto">
        </div>
        <h1 class="text-2xl font-bold text-center mb-4">Hey Rhoda ❤ </h1>
        <p class="text-gray-700 text-center mb-4">I made this little card to let you know how special you are. 😊</p>
        <div class="flex justify-center">
            <button id="revealButton" class="bg-blue-500 text-white px-4 py-2 rounded hover:bg-blue-700">Click !</button>
        </div>
        <div id="hiddenMessage" class="hidden-message mt-4 text-center text-lg text-gray-800">
            <p> can i be your dog 🐶</p>
        </div>
    </div>

    <script>
        document.getElementById('revealButton').addEventListener('click', function () {
            var hiddenMessage = document.getElementById('hiddenMessage');
            hiddenMessage.classList.toggle('visible-message');
        });
    </script>
</body>

</html>
