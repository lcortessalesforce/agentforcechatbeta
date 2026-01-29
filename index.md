<html lang="en">
<head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>Agentforce Help</title>
    <style>

/* General body and header styles */
body {
    margin: 0;
    font-family: Arial, sans-serif;
    background: linear-gradient(to bottom, #e9f1ff, #f9faff);
}

header nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 10px 20px;
    background-color: #fff;
    box-shadow: 0px 2px 5px rgba(0, 0, 0, 0.1);
}

header nav a {
    text-decoration: none;
    color: #333;
    margin-right: 15px;
    font-size: 14px;
}

.contact-support {
    padding: 5px 10px;
    background-color: #007BFF;
    color: #fff;
    border: none;
    border-radius: 3px;
    cursor: pointer;
}

.contact-support:hover {
    background-color: #0056b3;
}

/* Hero section styles */
main .hero {
    text-align: center;
    padding: 100px 20px;
    background: linear-gradient(to bottom, #eaf3ff, #ffffff);
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
}

.robot-icon {
    width: 100px;
    margin-bottom: 20px;
}

h1 {
    font-size: 36px;
    color: #333;
}

.brand {
    color: #007BFF;
}

.search-bar {
    margin-top: 20px;
}

.search-bar input {
    padding: 10px;
    width: 60%;
    max-width: 500px;
    border: 1px solid #ccc;
    border-radius: 5px;
    font-size: 16px;
}

.search-bar .search-btn {
    padding: 10px 20px;
    background-color: #007BFF;
    color: white;
    border: none;
    border-radius: 5px;
    font-size: 16px;
    cursor: pointer;
    margin-left: -5px;
}

.search-bar .search-btn:hover {
    background-color: #0056b3;
}

/* Chat modal styles */
#embeddedMessagingContainer {
    display: none; /* Initially hidden */
    position: fixed;
    top: 0;
    left: 0;
    z-index: 1000;
    width: 100vw;
    height: 100vh;
    background: rgba(255, 255, 255, 0.95);
    box-shadow: 0px 2px 10px rgba(0, 0, 0, 0.3);
}

#embeddedMessagingContainer.show {
    display: flex;
    justify-content: center;
    align-items: center;
}

#embedded-messaging, #embeddedMessagingFrame {
    height: 90%;
    width: 90%;
    border-radius: 10px;
}

#embeddedMessagingFrame {
    box-shadow: none;
}

#embeddedMessagingConversationButton {
    display: none;
}
      
    </style>
</head>
<body>
    <header>
        <nav>
            <a href="#">Help</a>
            <a href="https://lcortessalesforce.github.io/agentforcechatbeta">Ask Agentforce</a>
            <a href="#">Product Documentation</a>
            <a href="#">Trailhead Learning</a>
            <a href="#">My Cases</a>
            <button class="contact-support">Contact Support</button>
        </nav>
    </header>
    <main>
        <div class="hero">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSC_QFbTFMasUfnuKan4pWGlVr4700Fo7_9-w&s" alt="Agentforce Robot" class="robot-icon" />
            <h1>How can <span class="brand">Agentforce</span> help?</h1>
            <div class="search-bar">
                <input id="queryInput" type="text" placeholder='Ask questions like "How do I reset my password?"'/>
                <button class="search-btn" onclick="return false;">🔍</button>
            </div>
        </div>
        <!-- Embedded Messaging Container -->
        <div id="embeddedMessagingContainer" class="chat-modal"></div>
    </main>

<script type='text/javascript' 
             id='init-agentforce-messaging' 
             src='https://test-service.force.com/embeddedservice/agentforcemessaging/0.3/init.js' 
             onload='agentforce_messaging.init({
                    siteUrl: "lcortessalesforce.github.io",
                    agentApiConfiguration: {
                        agentId: "0XxWs000000wU0vKAE", 
                        domainUrl: "https://storm-001a1a6640a1b1--pro.sandbox.my.salesforce.com"
                    },
                    uiConfiguration: {}
            });'>
</script>

    </body>
  </html>
