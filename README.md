# Whatsapp-mejorado
/* Contenedor principal */
.whatsapp-container {
    display: grid;
    grid-template-columns: 30% 70%;
    height: 100vh;
    font-family: 'Arial', sans-serif;
}

/* Barra de búsqueda */
.search-bar {
    padding: 10px;
    background-color: var(--bg-light);
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.search-bar input {
    width: 100%;
    padding: 10px;
    border: none;
    border-radius: 5px;
    background-color: var(--bg-input);
    font-size: 14px;
    transition: box-shadow 0.3s;
}

.search-bar input:focus {
    box-shadow: 0 0 5px rgba(0, 123, 255, 0.5);
    outline: none;
}

/* Lista de chats */
.chat-list {
    background-color: var(--bg-light);
    overflow-y: auto;
    border-right: 1px solid #ddd;
}

.chat {
    display: flex;
    align-items: center;
    padding: 10px;
    cursor: pointer;
    transition: background-color 0.3s;
}

.chat:hover {
    background-color: var(--bg-hover);
}

.profile-pic {
    width: 40px;
    height: 40px;
    border-radius: 50%;
    margin-right: 10px;
}

.chat-info h4 {
    margin: 0;
    font-size: 16px;
    color: var(--text-dark);
}

.chat-info p {
    margin: 0;
    font-size: 14px;
    color: var(--text-muted);
}

.time {
    margin-left: auto;
    font-size: 12px;
    color: var(--text-muted);
}

/* Ventana de mensajes */
.message-window {
    padding: 20px;
    background-color: var(--bg-main);
    display: flex;
    flex-direction: column;
    gap: 10px;
    overflow-y: auto;
}

.message {
    max-width: 60%;
    padding: 10px;
    border-radius: 10px;
    font-size: 14px;
}

.message.received {
    background-color: var(--bg-received);
    align-self: flex-start;
}

.message.sent {
    background-color: var(--bg-sent);
    color: white;
    align-self: flex-end;
}

/* Temas */
:root {
    --bg-light: #f5f5f5;
    --bg-main: #e5ddd5;
    --bg-input: #ffffff;
    --bg-hover: #ebebeb;
    --bg-received: #ffffff;
    --bg-sent: #25d366;
    --text-dark: #000000;
    --text-muted: #555555;
}

.dark-theme {
    --bg-light: #2a2f32;
    --bg-main: #121b22;
    --bg-input: #202c33;
    --bg-hover: #314145;
    --bg-received: #1e2d34;
    --bg-sent: #056162;
    --text-dark: #e9edef;
    --text-muted: #8696a0;
}
