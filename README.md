# 🦅 TURBO[ THE TREVINO DOCTRINE v42.2 ] 🦅

## THE MISSION
Fuck MetroPCS hotspot data limits. This isn't some boot-see workaround; this is a Sand Hill Road-level network architecture engineered to route your PC's entire network stack through your Android device via an ADB SOCKS5 tunnel. 

When executed correctly, your PC gets unlimited, unthrottled internet straight from your phone's primary data plan. No hotspot data consumed.

## THE PREREQUISITES (THE INTEL)
Before you even touch the script, get your shit right:
1. **Developer Options & USB Debugging:** Must be ENABLED on your Android phone.
2. **Every Proxy (App):** Download and install "Every Proxy" from the Play Store.
3. **The Hardline:** Connect your phone to your PC via a high-quality USB cable.

---

## THE EXECUTION PLAYBOOK (STEP-BY-STEP)

If you fuck up the sequence, the tunnel collapses. Follow the logic exactly. The script requires you to press `ENTER` to execute each strike step-by-step. Read the output. 

### PHASE 1: THE CLEAN SLATE (NUKE)
You cannot build a flawless system on a dirty foundation. We start by scrubbing the network state.
1. Run the script: `sudo ./turbo`
2. Select Option **4[ NUKE ]**.
3. Press `ENTER` to step through the commands. This kills old daemons, flushes IP tables, and scrubs the ghosts. 
4. **CRITICAL:** The final command in this sequence starts the ADB server. **Look at your phone.** A prompt will pop up asking to allow USB Debugging from this computer's RSA key. 
5. **Check the box** that says "Always allow from this computer" and hit **Allow**. 

### PHASE 2: THE PAYLOAD (EVERY PROXY)
Now that the PC and phone are officially shaking hands, we stand up the proxy server on the phone.
1. Open the **Every Proxy** app on your phone.
2. Toggle on the **SOCKS5** proxy.
3. Ensure the port is set exactly to: `1081`.
4. Leave it running on your phone screen. 

### PHASE 3: THE WELD (TURBO)
This is where the magic happens. We bind the local port, build the TUN interface, and force all PC traffic through the phone.
1. Go back to the script's main menu.
2. Select Option **1 [ TURBO ]**.
3. Press `ENTER` to execute each strike. The system will mangle the TTL, kill the DNS backdoors, launch `tun2socks`, and lock the traffic into the tunnel.

### PHASE 4: THE PHANTOM (GHOST)
NetworkManager will try to trip you up if it doesn't see a "real" connection. We deploy a dummy interface to keep it quiet.
1. Go back to the script's main menu.
2. Select Option **2 [ GHOST ]**.
3. Press `ENTER` to execute the strikes. This spins up the `nm-ghost` hardware interface.

### PHASE 5: HOLD THE LINE
**DO NOT CLOSE THE SCRIPT.** 
Leave the terminal window open and running. The tunnel is live. The system is locked. Open your browser and enjoy your unthrottled, unlimited data. 

To tear down the tunnel and return to normal, go back to the script and hit Option **4 [ NUKE ]**.
