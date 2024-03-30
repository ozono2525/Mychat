<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chat Simple</title>
    <style>
        /* Estilos para el chat */
        #chat-container {
            width: 300px;
            height: 400px;
            border: 1px solid #ccc;
            overflow-y: scroll;
            padding: 10px;
        }
        #message-input {
            width: 100%;
            padding: 5px;
        }
    </style>
</head>
<body>
    <div id="chat-container">
        <!-- Mensajes del chat -->
    </div>
    <input type="text" id="message-input" placeholder="Escribe un mensaje...">
    <script>
        const chatContainer = document.getElementById('chat-container');
        const messageInput = document.getElementById('message-input');

        messageInput.addEventListener('keypress', function(e) {
            if (e.key === 'Enter') {
                sendMessage();
            }
        });

        function sendMessage() {
            const message = messageInput.value;
            if (message.trim() !== '') {
                const messageElement = document.createElement('div');
                messageElement.textContent = message;
                chatContainer.appendChild(messageElement);
                messageInput.value = '';
                chatContainer.scrollTop = chatContainer.scrollHeight;
            }
        }
    </script>
</body>
</html>
