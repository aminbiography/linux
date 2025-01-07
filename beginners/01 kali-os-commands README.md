


<h1>Open Terminal in Kali Linux</h1>
<h3>Keyboard Shortcut:</h3>
<p>Press <strong>"Ctrl + Alt + T"</strong> to open the terminal.</p>

<h3>Through GUI:</h3>
<ul>
    <li>Click on the <strong>Applications</strong> menu in the top-left corner.</li>
    <li>Navigate to <strong>System Tools</strong>.</li>
    <li>Select <strong>Terminal</strong>.</li>
</ul>


===================================================================================================================================================================

<h1>Maximize and Minimize the Kali Linux Terminal</h1>

<p>You can maximize or minimize the Kali Linux terminal using a combination of <strong>keyboard shortcuts</strong>, <strong>mouse actions</strong>, or <strong>terminal commands</strong>, depending on your desktop environment (e.g., GNOME, XFCE).</p>

<h3>Using the Mouse</h3>

<h4>Maximize the Terminal:</h4>
<ul>
    <li>Click the <strong>maximize</strong> button (usually located in the top-right or top-left corner of the terminal window).</li>
    <li>Alternatively, drag the terminal window to the top edge of the screen to maximize it (depending on your desktop environment).</li>
</ul>

<h4>Minimize the Terminal:</h4>
<ul>
    <li>Click the <strong>minimize</strong> button (usually located next to the maximize button).</li>
    <li>Alternatively, right-click the terminal in the taskbar and select <strong>Minimize</strong>.</li>
</ul>

<hr>

<h3>Using Keyboard Shortcuts</h3>

<h4>For GNOME (default Kali desktop):</h4>
<ul>
    <li><strong>Maximize the Terminal:</strong> Press <code>Super</code> (Windows key) + <code>↑</code> (up arrow).</li>
    <li><strong>Minimize the Terminal:</strong> Press <code>Super</code> (Windows key) + <code>↓</code> (down arrow).</li>
</ul>

<h4>For XFCE:</h4>
<ul>
    <li><strong>Maximize the Terminal:</strong> Press <code>Alt + F10</code>.</li>
    <li><strong>Minimize the Terminal:</strong> Press <code>Alt + F9</code>.</li>
</ul>

<hr>

<h3>Using Terminal Commands</h3>
<p>You can also control the terminal window from the command line using tools like <code>xdotool</code> (if installed).</p>

<h4>Maximize:</h4>
<pre><code>xdotool getactivewindow windowsize 100% 100%</code></pre>

<h4>Minimize:</h4>
<pre><code>xdotool getactivewindow windowminimize</code></pre>

<p><strong>Note:</strong> You may need to install <code>xdotool</code> using the following command if it's not already installed:</p>
<pre><code>sudo apt install xdotool</code></pre>

<hr>

<h3>Full-Screen Mode</h3>

<h4>Enter Full-Screen Mode:</h4>
<ul>
    <li>Press <code>F11</code> (works in most terminal emulators like GNOME Terminal or XFCE Terminal).</li>
</ul>

<h4>Exit Full-Screen Mode:</h4>
<ul>
    <li>Press <code>F11</code> again.</li>
</ul>

===================================================================================================================================================================
<h1>Check System Status in Kali Linux</h1>

<p>To quickly check the system's overall status in Kali Linux, use the following command:</p>
    
<pre><code>
sudo systemctl is-system-running
</code></pre>

<p>The output will be concise and indicate the current system status. Example:</p>

<pre>
running
</pre>

<p>This command provides a one-word summary of the system's health:</p>
<ul>
    <li><strong>running</strong>: The system is operating normally.</li>
    <li><strong>degraded</strong>: Some services have failed but the system is functional.</li>
    <li><strong>maintenance</strong>: The system is in maintenance mode.</li>
    <li><strong>failed</strong>: A critical issue has occurred.</li>
</ul>

<p>This is an efficient way to perform a quick health check on your Linux system.</p>
===================================================================================================================================================================

<h1>Closing Terminal in Kali Linux</h1>
<h3>Keyboard Shortcut:</h3>
<p>Press <strong>"Ctrl + D"</strong> to close the terminal.</p>

<h3>Through GUI:</h3>
<ul>
    <li>Click the <strong>Close</strong> button (X) on the terminal window.</li>
    <li>Or right-click the terminal icon and select <strong>Close</strong>.</li>
</ul>

<h1>OS Shutdown Commands in Kali Linux</h1>
<h3>Immediate Shutdown (Admin Privileges Required):</h3>
<pre><code>sudo shutdown now</code></pre>

<h3>Scheduled Shutdown:</h3>
<pre><code>sudo shutdown +&lt;time&gt;</code></pre>

<h3>Shutdown with a Custom Message:</h3>
<pre><code>sudo shutdown +5 "System is shutting down for maintenance."</code></pre>

<h3>Power Off Directly:</h3>
<pre><code>sudo poweroff</code></pre>

<h3>Reboot Command (Optional for Restart):</h3>
<pre><code>sudo reboot</code></pre>

<h3>Halt the System (Stop All Processes):</h3>
<pre><code>sudo halt</code></pre>

<h3>Notes:</h3>
<ul>
    <li>Always use <strong>"sudo"</strong> because shutting down typically requires administrator privileges.</li>
    <li>If you're logged in as the <strong>root user</strong>, you can skip <strong>"sudo"</strong>.</li>
    <li>For GUI users, you can also shut down using the <strong>menu options</strong> or <strong>power button</strong>.</li>
</ul>









