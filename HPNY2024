<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Which Red Envelope do you want? :3</title>
    <style>
        body {
            background-color: #ffd699; /* Light Orange background */
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            margin: 0;
            font-family: 'Arial', sans-serif;
        }

        h1 {
            color: #000000; /* Black text color */
            font-weight: bold;
        }

        .red-envelope-container {
            position: relative;
            display: flex;
            gap: 20px;
            justify-content: center;
            align-items: center;
        }

        .red-envelope {
            width: 150px;
            height: 200px;
            background-color: #ff4d4d;
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #ffffff;
            font-size: 20px;
            font-weight: bold;
            text-align: center;
            cursor: pointer;
            transition: transform 0.3s ease-in-out;
            animation: envelopeAnimation 2s infinite alternate;
        }

        @keyframes envelopeAnimation {
            0% {
                transform: translateY(0);
            }
            100% {
                transform: translateY(-10px);
            }
        }

        .red-envelope:hover {
            transform: scale(1.05);
            animation: none; /* Pause animation on hover */
        }

        #congratulations {
            display: none;
            font-size: 24px;
            font-weight: bold;
            color: #000000; /* Black text color */
            text-align: center;
            margin-top: 20px;
        }

        #how-to-get-it-button {
            display: none;
            background-color: #cc3300; /* Dark Orange button color */
            color: #ffffff;
            border: none;
            padding: 10px;
            border-radius: 5px;
            cursor: pointer;
        }

        #how-to-get-it-content {
            display: none;
            margin-top: 20px;
            font-size: 16px;
            text-align: center;
        }
    </style>
</head>
<body>

    <h1>Which Red Envelope do you want? :3</h1>

    <div class="red-envelope-container">
        <div class="red-envelope" onclick="showCongratulations(3000000)">?</div>
        <div class="red-envelope" onclick="showCongratulations(8000000)">?</div>
        <div class="red-envelope" onclick="showCongratulations(10000000)">?</div>
        <div class="red-envelope" onclick="showCongratulations(13000000)">?</div>
	<div class="red-envelope" onclick="showCongratulations(15000000)">?</div>
    </div>

    <div id="congratulations"></div>
    <button id="how-to-get-it-button" onclick="showHowToGetIt()">How to get it</button>
    <div id="how-to-get-it-content"></div>

    <script>
        function showCongratulations(amount) {
            var congratulationsElement = document.getElementById('congratulations');
            congratulationsElement.innerText = `Congratulations! You've chosen a ${amount}VND red envelope!`;
            congratulationsElement.style.display = 'block';

            // Show "How to get it" button after 1 second
            setTimeout(function () {
                var howToGetItButton = document.getElementById('how-to-get-it-button');
                howToGetItButton.style.display = 'block';
            }, 1000);
        }

        function showHowToGetIt() {
            var howToGetItContentElement = document.getElementById('how-to-get-it-content');

            var selectedAmount = document.getElementById('congratulations').innerText.match(/\d+/)[0];

            switch (parseInt(selectedAmount)) {
                case 3000000:
                    howToGetItContentElement.innerHTML = "Refer <strong>Standard/Standard++/PMA</strong> candidate to <strong>career@nfq.com</strong> or to <strong>anh.le</strong> (Slack)";
                    break;
                case 8000000:
                    howToGetItContentElement.innerHTML = "Refer <strong>PM/Senior PM</strong> candidate to <strong>career@nfq.com</strong> or to <strong>anh.le</strong> (Slack)";
                    break;
                case 10000000:
                    howToGetItContentElement.innerHTML = "Refer <strong>Senior/Senior++</strong> candidate to <strong>career@nfq.com</strong> or to <strong>anh.le</strong> (Slack)";
                    break;
                case 13000000:
                    howToGetItContentElement.innerHTML = "Refer <strong>Lead</strong> candidate to <strong>career@nfq.com</strong> or to <strong>anh.le</strong> (Slack)";
		    break;
                case 15000000:
                    howToGetItContentElement.innerHTML = "Refer <strong>Technical Architect</strong> candidate to <strong>career@nfq.com</strong> or to <strong>anh.le</strong> (Slack)";
                    break;
                default:
                    howToGetItContentElement.innerText = "Refer candidate to career@nfq.com or to anh.le (Slack)";
                    break;
            }

            // Display "How to get it" content
            howToGetItContentElement.style.display = 'block';

            // Hide "How to get it" button
            var howToGetItButton = document.getElementById('how-to-get-it-button');
            howToGetItButton.style.display = 'none';
        }
    </script>

</body>
</html>
