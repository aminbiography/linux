

<h1>How to Update Kali Linux</h1>

<h2>Steps to Run <code>apt update</code> in Kali Linux</h2>

<ol>
  <li>
    <strong>Open a Terminal</strong><br />
    Press <code>Ctrl + Alt + T</code> or search for "Terminal" in the applications menu.
  </li>
  <li>
    <strong>Run as Root</strong><br />
    Either switch to the root user using:
    <pre><code>sudo -i</code></pre>
    or prefix commands with <code>sudo</code>.
  </li>
  <li>
    <strong>Update the Package List</strong><br />
    Run the following command:
    <pre><code>sudo apt update</code></pre>
  </li>
  <li>
    <strong>Upgrade Installed Packages</strong> (Optional but Recommended)<br />
    Upgrade installed packages to the latest versions:
    <pre><code>sudo apt upgrade -y</code></pre>
  </li>
  <li>
    <strong>Perform a Dist-Upgrade</strong> (Optional)<br />
    Handle upgrades involving dependency changes or obsolete packages:
    <pre><code>sudo apt dist-upgrade -y</code></pre>
  </li>
  <li>
    <strong>Clean Up Unused Files</strong> (Optional)<br />
    Remove unnecessary packages and clean up:
    <pre><code>sudo apt autoremove -y
sudo apt autoclean</code></pre>
  </li>
</ol>

<h2>Common Errors and Fixes</h2>

<ul>
  <li>
    <strong>Key Issues:</strong><br />
    If you encounter issues with missing public keys, run:
    <pre><code>sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys [KEY_ID]</code></pre>
    Replace <code>[KEY_ID]</code> with the missing key's ID from the error message.
  </li>
  <li>
    <strong>Repository Errors:</strong><br />
    Ensure the <code>/etc/apt/sources.list</code> file is properly configured. For Kali Linux, a typical <code>sources.list</code> file includes:
    <pre><code>deb http://http.kali.org/kali kali-rolling main contrib non-free</code></pre>
    To edit this file:
    <pre><code>sudo nano /etc/apt/sources.list</code></pre>
  </li>
</ul>

<p>After making any changes, re-run <code>sudo apt update</code>.</p>
