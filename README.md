# Smmking <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SMM Bot Setup Guide</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        .code-block {
            font-family: 'Courier New', monospace;
            background-color: #2d3748;
            color: #f7fafc;
            border-radius: 0.375rem;
            padding: 1rem;
            position: relative;
        }
        .copy-btn {
            position: absolute;
            top: 0.5rem;
            right: 0.5rem;
            background-color: #4a5568;
            color: white;
            border: none;
            border-radius: 0.25rem;
            padding: 0.25rem 0.5rem;
            cursor: pointer;
            transition: all 0.2s;
        }
        .copy-btn:hover {
            background-color: #718096;
        }
        .step-icon {
            background-color: #4299e1;
            color: white;
            border-radius: 9999px;
            width: 2.5rem;
            height: 2.5rem;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-right: 1rem;
            flex-shrink: 0;
        }
    </style>
</head>
<body class="bg-gray-100 min-h-screen">
    <div class="container mx-auto px-4 py-8 max-w-4xl">
        <div class="bg-white rounded-lg shadow-lg overflow-hidden">
            <!-- Header -->
            <div class="bg-blue-600 p-6 text-white">
                <div class="flex items-center">
                    <i class="fas fa-robot text-4xl mr-4"></i>
                    <div>
                        <h1 class="text-2xl font-bold">SMM Bot Setup Guide</h1>
                        <p class="opacity-90">Follow these steps to install and run the SMM automation tool</p>
                    </div>
                </div>
            </div>
            
            <!-- Content -->
            <div class="p-6">
                <!-- Prerequisites -->
                <div class="mb-8">
                    <h2 class="text-xl font-semibold mb-4 text-gray-800 border-b pb-2">Prerequisites</h2>
                    <ul class="space-y-3">
                        <li class="flex items-start">
                            <i class="fas fa-check-circle text-green-500 mt-1 mr-2"></i>
                            <span>Git installed on your system (<a href="https://git-scm.com/downloads" class="text-blue-600 hover:underline" target="_blank">Download Git</a>)</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-check-circle text-green-500 mt-1 mr-2"></i>
                            <span>Python 3.6 or higher installed (<a href="https://www.python.org/downloads/" class="text-blue-600 hover:underline" target="_blank">Download Python</a>)</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-check-circle text-green-500 mt-1 mr-2"></i>
                            <span>Basic knowledge of command line/terminal</span>
                        </li>
                    </ul>
                </div>
                
                <!-- Installation Steps -->
                <div class="mb-8">
                    <h2 class="text-xl font-semibold mb-4 text-gray-800 border-b pb-2">Installation Steps</h2>
                    
                    <!-- Step 1 -->
                    <div class="flex mb-6">
                        <div class="step-icon">
                            <span class="font-bold">1</span>
                        </div>
                        <div class="flex-1">
                            <h3 class="font-medium text-lg mb-2">Clone the Repository</h3>
                            <p class="text-gray-600 mb-3">Open your terminal/command prompt and run:</p>
                            <div class="code-block mb-3">
                                <button class="copy-btn" onclick="copyToClipboard('git clone https://github.com/Lariot08/SMM')">
                                    <i class="fas fa-copy"></i>
                                </button>
                                <code>git clone https://github.com/Lariot08/SMM</code>
                            </div>
                            <p class="text-gray-600 text-sm">This will download the SMM bot to your local machine.</p>
                        </div>
                    </div>
                    
                    <!-- Step 2 -->
                    <div class="flex mb-6">
                        <div class="step-icon">
                            <span class="font-bold">2</span>
                        </div>
                        <div class="flex-1">
                            <h3 class="font-medium text-lg mb-2">Navigate to the Directory</h3>
                            <p class="text-gray-600 mb-3">Change into the project directory:</p>
                            <div class="code-block mb-3">
                                <button class="copy-btn" onclick="copyToClipboard('cd SMM')">
                                    <i class="fas fa-copy"></i>
                                </button>
                                <code>cd SMM</code>
                            </div>
                        </div>
                    </div>
                    
                    <!-- Step 3 -->
                    <div class="flex mb-6">
                        <div class="step-icon">
                            <span class="font-bold">3</span>
                        </div>
                        <div class="flex-1">
                            <h3 class="font-medium text-lg mb-2">Run the Bot</h3>
                            <p class="text-gray-600 mb-3">Execute the Python script to start the bot:</p>
                            <div class="code-block mb-3">
                                <button class="copy-btn" onclick="copyToClipboard('python bot.py')">
                                    <i class="fas fa-copy"></i>
                                </button>
                                <code>python bot.py</code>
                            </div>
                            <p class="text-gray-600 text-sm">Note: You might need to use <code class="bg-gray-200 px-1 py-0.5 rounded">python3</code> instead of <code class="bg-gray-200 px-1 py-0.5 rounded">python</code> on some systems.</p>
                        </div>
                    </div>
                </div>
                
                <!-- Troubleshooting -->
                <div class="bg-yellow-50 border-l-4 border-yellow-400 p-4 mb-6">
                    <div class="flex">
                        <div class="flex-shrink-0">
                            <i class="fas fa-exclamation-triangle text-yellow-400 mt-1 mr-3"></i>
                        </div>
                        <div>
                            <h3 class="text-sm font-medium text-yellow-800">Troubleshooting</h3>
                            <div class="mt-2 text-sm text-yellow-700">
                                <p>If you encounter any issues:</p>
                                <ul class="list-disc pl-5 space-y-1 mt-1">
                                    <li>Make sure all dependencies are installed (check requirements.txt)</li>
                                    <li>Ensure Python is in your system PATH</li>
                                    <li>Run the command prompt/terminal as administrator if needed</li>
                                </ul>
                            </div>
                        </div>
                    </div>
                </div>
                
                <!-- Additional Info -->
                <div class="bg-blue-50 border-l-4 border-blue-400 p-4">
                    <div class="flex">
                        <div class="flex-shrink-0">
                            <i class="fas fa-info-circle text-blue-400 mt-1 mr-3"></i>
                        </div>
                        <div>
                            <h3 class="text-sm font-medium text-blue-800">Additional Information</h3>
                            <div class="mt-2 text-sm text-blue-700">
                                <p>For more details about this project, visit the <a href="https://github.com/Lariot08/SMM" class="font-medium underline hover:text-blue-600" target="_blank">GitHub repository</a>.</p>
                                <p class="mt-1">Make sure to read any README or documentation files included with the project.</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- Footer -->
            <div class="bg-gray-100 px-6 py-4 border-t">
                <div class="flex justify-between items-center">
                    <p class="text-gray-600 text-sm">SMM Automation Tool</p>
                    <div class="flex space-x-4">
                        <a href="#" class="text-gray-500 hover:text-gray-700">
                            <i class="fab fa-github"></i>
                        </a>
                        <a href="#" class="text-gray-500 hover:text-gray-700">
                            <i class="fab fa-python"></i>
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <script>
        function copyToClipboard(text) {
            navigator.clipboard.writeText(text).then(function() {
                // Show a temporary tooltip or notification
                const btn = event.target.closest('button');
                const originalHTML = btn.innerHTML;
                btn.innerHTML = '<i class="fas fa-check"></i>';
                btn.style.backgroundColor = '#48bb78';
                
                setTimeout(() => {
                    btn.innerHTML = originalHTML;
                    btn.style.backgroundColor = '#4a5568';
                }, 2000);
            }, function(err) {
                console.error('Could not copy text: ', err);
            });
        }
    </script>
</body>
</html>
