<!DOCTYPE html>
<html lang="de">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover" />
<title>Wimmelbild – Plan:g (Mobile)</title>
<link rel="icon" type="image/png" href="favicon.png" />
<script src="./openseadragon/openseadragon.min.js"></script>

<style>
  :root{
    --green:#789f40;
    --green-dark:#769b60;
    --accent:#870184;
    --bg:#f3f3f3;
    --pad: clamp(14px, 4vw, 20px);
    --hotspot-color:#ffffff;
    --hotspot-border:rgba(0,0,0,.25);
  }
  *,*::before,*::after{ box-sizing:border-box; }
  html,body{ margin:0; background:var(--bg); font-family: system-ui,-apple-system,Segoe UI,Roboto,Arial,sans-serif; color:#111; }
  a{ color:inherit; text-decoration:none; }

  /* Header + Abstände */
  .m-header{ padding: calc(env(safe-area-inset-top) + 14px) var(--pad) 16px; }
  .m-header__logo{ width: clamp(150px, 48vw, 220px); height:auto; display:block; }

  .cta{
    margin-top:10px; font-weight:700; text-transform:uppercase;
    font-size:clamp(13px,3.7vw,16px);
    background:var(--green); color:#fff;
    padding:12px 16px; border-radius:14px;
    display:inline-flex; align-items:center; justify-content:center;
    box-shadow:0 2px 8px rgba(0,0,0,.12);
  }
  .cta.square{ border-radius:0; }
  .cta:active{ transform:scale(.98); }
  .m-ctas{ margin-top:14px; display:grid; gap:12px; max-width:360px; }

  .m-headline{ padding:12px var(--pad) 0; margin-bottom: clamp(14px, 4vw, 26px); }
  .m-headline h1{ margin:0; font-size:clamp(18px,5.2vw,22px); line-height:1.28; }

  .circle-wrap{
    padding: clamp(22px, 4.8vw, 32px) var(--pad) clamp(14px, 3.6vw, 24px);
    display:grid; place-items:center;
  }
  .circle{
    width:min(86vw,520px); aspect-ratio:1/1; border-radius:0;
    clip-path:circle(50% at 50% 50%); background:var(--green-dark);
    overflow:hidden; position:relative; box-shadow:0 8px 28px rgba(0,0,0,.18);
  }
  .circle.is-fullscreen{ clip-path:none; border-radius:0; width:100vw; height:100vh; background:#000; }
  .pseudo-fs .circle{ clip-path:none!important; border-radius:0!important; position:fixed!important; inset:0!important; width:100vw!important; height:100vh!important; background:#000!important; z-index:998!important; }

  #myContainer{ position:absolute; inset:0; width:100%; height:100%; background:transparent; touch-action:manipulation; z-index:1; }

  /* Herz oben rechts */
  .heart-cta{
    position:absolute; top:12px; right:12px; z-index:1000;
    display:block; opacity:1;
  }
  .heart-cta img{ display:block; width: clamp(24px, 6vw, 44px); height:auto; }

  /* Hotspots */
  .hotspot-overlay{
    width:20px; height:20px;
    background:var(--hotspot-color);
    background-size:contain; background-position:center; background-repeat:no-repeat;
    border:1px solid var(--hotspot-border);
    border-radius:0;
    box-shadow:0 1px 4px rgba(0,0,0,.35);
    cursor:pointer; touch-action:manipulation; opacity:1; z-index:2;
    transition:opacity .15s ease;
    -webkit-tap-highlight-color: rgba(0,0,0,0);
  }
  .hotspot-overlay.has-icon{
    appearance:none; -webkit-appearance:none;
    padding:0;
    background-color:transparent !important;
    border:0 !important;
    box-shadow:none !important;
    outline:none !important;
    border-radius:9999px !important;
    overflow:hidden;
    background-clip:padding-box;
  }
  .hotspot-overlay.has-icon:focus,
  .hotspot-overlay.has-icon:focus-visible,
  .hotspot-overlay.has-icon:active{
    outline:none !important;
    background-color:transparent !important;
    border:0 !important;
    box-shadow:none !important;
  }
  .hotspot-overlay.is-hidden{ opacity:0; pointer-events:none; }

  .circle.is-fullscreen .hotspot-overlay,
  .pseudo-fs .hotspot-overlay{ opacity:1; border-width:1px; box-shadow:0 1px 3px rgba(0,0,0,.3); }

  /* Popup (nur Bild) */
  .popup{
    background:transparent; padding:0; border:none; border-radius:0; box-shadow:none;
    overflow:visible; max-width:90vw; max-height:85vh; z-index:3;
  }
  .circle.is-fullscreen .popup{ max-width:90vw; max-height:85vh; }
  .popup img{ display:block; width:auto; height:auto; max-width:100%; max-height:100%; object-fit:contain; border-radius:0; }

  .m-footer{ padding:12px var(--pad) calc(env(safe-area-inset-bottom) + 18px); display:grid; gap:8px; }
  .language{ display:flex; gap:12px; align-items:center; }
  .flag{ width:28px; height:21px; background-size:cover; background-repeat:no-repeat; border-radius:3px; box-shadow:0 1px 3px rgba(0,0,0,.2); }
  .flag.de{ background-image:url("https://cdnjs.cloudflare.com/ajax/libs/flag-icon-css/3.2.1/flags/4x3/at.svg"); }
  .flag.en{ background-image:url("https://cdnjs.cloudflare.com/ajax/libs/flag-icon-css/3.2.1/flags/4x3/gb.svg"); }
  .text-link{ color:var(--green); }
  .m-footer p{ margin:0; font-size:14px; }
</style>
</head>

<body>
  <header class="m-header">
    <img src="img/logo.png" alt="Plan:g – logo" class="m-header__logo" />
    <div class="m-ctas">
      <a href="https://plan-g.at/fachthemen/medizin-und-eza" target="_blank" rel="noopener" class="cta square">Dieses Poster</a>
      <a href="https://plan-g.at/projekte/alle-projekte" target="_blank" rel="noopener" class="cta square">Unsere Arbeit</a>
      <a href="https://plan-g.at/news-events/informiert-bleiben" target="_blank" rel="noopener" class="cta square">Informiert bleiben</a>
    </div>
  </header>

  <section class="m-headline">
    <h1>
      Die Welt ist ziemlich klein,<br />
      Gesundheit ziemlich komplex:<br />
      Viel Spaß beim Entdecken.
    </h1>
  </section>

  <section class="circle-wrap" aria-label="Interaktives Wimmelbild">
    <div class="circle" id="circle">
      <!-- Viewer -->
      <div id="myContainer" role="application" aria-label="Wimmelbild Viewer"></div>

      <!-- Herz oben rechts -->
      <a class="heart-cta" href="https://plan-g.at/ueber-uns" target="_blank" rel="noopener" aria-label="Über uns">
        <img src="img/signet_bunt.png" alt="" />
      </a>
    </div>
  </section>

  <footer class="m-footer">
    <div class="language">
      <a href="https://weltgesundheit.org" class="text-link" aria-label="Deutsch"><div class="flag de" title="Deutsch"></div></a>
      <a href="https://weltgesundheit.org/en/" class="text-link" aria-label="English"><div class="flag en" title="English"></div></a>
    </div>
    <p>Illustration: Alice Ruzzettu</p>
    <a href="http://plan-g.at/impressum" class="text-link" target="_blank" rel="noopener">Impressum</a>
  </footer>

<script>
  /* ====== Pfade ====== */
  const ASSETS_BASE = "./Assets";
  const ICON_DEFAULT = `${ASSETS_BASE}/button-wim.png`;
  const POPUPS_DIRS = [`${ASSETS_BASE}/popups`, `${ASSETS_BASE}/popups-2`];

  /* ====== OpenSeadragon ====== */
  const viewer = OpenSeadragon({
    id: "myContainer",
    prefixUrl: "openseadragon/images/",
    tileSources: {
      type: "image",
      width: 5787,
      height: 7722,
      url: "./img/wimmelbildfinal.jpg",
      minLevel: 0,
      maxLevel: 5,
      buildPyramid: true
    },
    showNavigator: false,
    showNavigationControl: true,     // zeigt Haus + Full-Page Button
    autoHideControls: true,
    blendTime: 0.12,
    animationTime: 0.85,
    springStiffness: 6.5,
    zoomPerClick: 1.22,
    zoomPerScroll: 1.14,
    visibilityRatio: 0.95,
    constrainDuringPan: true,
    minZoomImageRatio: 1,
    maxZoomPixelRatio: 2.0,
    immediateRender: true
  });

  /* ====== Größen/Koordinaten ====== */
  const SOURCE_W = 5787, SOURCE_H = 7722;
  const AUTHOR_W = 14344, AUTHOR_H = 19140;
  const Y_EXTRA_SCALE = 1.3348;
  function normalizeXY(xAuthor, yAuthor) {
    const nx = (xAuthor * (SOURCE_W / AUTHOR_W)) / SOURCE_W;
    const ny = (yAuthor * (SOURCE_H / AUTHOR_H)) / SOURCE_H * Y_EXTRA_SCALE;
    return { nx, ny };
  }

  /* ====== Responsive Hotspot-Größe ====== */
  function getHotspotSizeParams(){
    if (window.matchMedia('(max-width: 640px)').matches) return { BASE: 14, MIN: 10, MAX: 18 };
    return { BASE: 20, MIN: 14, MAX: 24 };
  }

  let osdIsFull = false;        // OSD FullPage/FullScreen Zustand (aus Events)
  let lastTapTs = 0;            // kleines Debounce für iOS (touchend + click)

  function applyHotspotScale(){
    const { BASE, MIN, MAX } = getHotspotSizeParams();
    const z = viewer.viewport.getZoom(true);
    const fs = (osdIsFull || document.body.classList.contains('pseudo-fs')) ? 0.98 : 1.0;
    const size = Math.max(MIN, Math.min(MAX, BASE * fs * (0.90 + (z-1)*0.12)));
    document.querySelectorAll('.hotspot-overlay').forEach(el => {
      el.style.width  = `${size}px`;
      el.style.height = `${size}px`;
    });
  }
  viewer.addHandler('zoom', applyHotspotScale);
  viewer.addHandler('resize', applyHotspotScale);
  viewer.addHandler('open', ()=>{ applyHotspotScale(); });

  /* ====== Vollbild-Logik: wir nutzen OSDs FullPage/FullScreen ====== */
  const circleEl    = document.getElementById('circle');
  const containerEl = document.getElementById('myContainer');

  function setFullscreenClasses(isFs){
    osdIsFull = !!isFs;
    circleEl.classList.toggle('is-fullscreen', osdIsFull);
    applyHotspotScale();
    updatePanBounds(osdIsFull);
  }
  function updatePanBounds(isFs){
    if (isFs || document.body.classList.contains('pseudo-fs')){
      viewer.constrainDuringPan = false;
      viewer.viewport.setVisibilityRatio(0.2);
      viewer.minZoomImageRatio = 0.8;
    } else {
      viewer.constrainDuringPan = true;
      viewer.viewport.setVisibilityRatio(0.95);
      viewer.minZoomImageRatio = 1;
    }
  }

  // OSD feuert zwei relevante Events:
  viewer.addHandler('full-page',  e => setFullscreenClasses(!!e.fullPage));
  viewer.addHandler('full-screen',e => setFullscreenClasses(!!e.fullScreen));

  // Falls Browser-Fullscreen doch genutzt wird (andere Controls o. Ä.)
  document.addEventListener('fullscreenchange', ()=>{
    const fs = !!(document.fullscreenElement || document.webkitFullscreenElement);
    setFullscreenClasses(fs);
  });
  document.addEventListener('webkitfullscreenchange', ()=>{
    const fs = !!(document.fullscreenElement || document.webkitFullscreenElement);
    setFullscreenClasses(fs);
  });

  // Tap/Klick → nur *einseitig* in FullPage gehen (kein Überschreiben des OSD-Buttons)
  async function ensureFullscreenIfNeeded(ev){
    const now = Date.now();
    if (now - lastTapTs < 300) return; // Debounce (iOS feuert oft touchend + click)
    lastTapTs = now;

    if (!osdIsFull){
      // bevorzugt OSD FullPage (stabil auf iOS)
      viewer.setFullPage(true);
      setFullscreenClasses(true);
    }
  }

  containerEl.addEventListener('touchend', (e)=>{
    if (e.touches && e.touches.length === 0){
      e.preventDefault();
      ensureFullscreenIfNeeded(e);
    }
  }, { passive:false });

  containerEl.addEventListener('click', (e)=>{
    ensureFullscreenIfNeeded(e);
  });

  /* ====== Popups/Hotspots ====== */
  let openPopupId = null;
  const popupTimers = new Map(); // id -> timeout

  function addOverlay(x, y, id, iconUrl, popupImage, popupText, popupTitle, colorValue, offsetX = 0, offsetY = 0) {
    const { nx, ny } = normalizeXY(x, y);
    const overlay = document.createElement("button");
    overlay.className = "hotspot-overlay";
    overlay.type = "button";
    overlay.setAttribute("aria-label", popupTitle || popupText || `Hotspot ${id}`);
    overlay.setAttribute("data-id", id);

    const finalIcon = iconUrl || ICON_DEFAULT;
    if (finalIcon) {
      overlay.classList.add("has-icon");
      overlay.style.backgroundImage = `url("${finalIcon}")`;
    } else if (colorValue) {
      overlay.style.setProperty("--hotspot-color", colorValue);
    }

    const open = async (e) => {
      e.stopPropagation(); e.preventDefault?.();
      await handleHotspotTap(nx, ny, id, popupImage, popupText, popupTitle, overlay, offsetX, offsetY);
    };
    overlay.addEventListener("touchend", open, { passive: false });
    overlay.addEventListener("click", open, { passive: true });

    viewer.addOverlay({
      element: overlay,
      location: new OpenSeadragon.Point(nx, ny),
      placement: OpenSeadragon.OverlayPlacement.CENTER
    });
  }

  async function handleHotspotTap(nx, ny, id, popupImage, popupText, popupTitle, overlayEl, offsetX = 0, offsetY = 0){
    if (!osdIsFull) viewer.setFullPage(true);
    focusOn(nx, ny, 1.6);

    if (openPopupId === id) { closePopup(id); return; }
    maybeOpenPopup(id, nx, ny, popupImage, popupText, popupTitle, overlayEl, true, offsetX, offsetY);
  }

  function resolvePopupSrc(name){
    if (!name) return null;
    if (name.includes("/")) return name;
    return `${POPUPS_DIRS[0]}/${name}`;
  }

  function maybeOpenPopup(id, x, y, popupImage, popupText, popupTitle, overlayEl, closeOthers=false, offsetX=0, offsetY=0){
    if (closeOthers && openPopupId && openPopupId !== id) closePopup(openPopupId);
    if (document.getElementById(`popup-${id}`)) return;

    if (overlayEl) overlayEl.classList.add('is-hidden');

    const imgSrc = resolvePopupSrc(popupImage);
    const popup = document.createElement("div");
    popup.className = "popup";
    popup.id = `popup-${id}`;
    popup.role = "dialog";
    popup.innerHTML = `${imgSrc ? `<img src="${imgSrc}" alt="" />` : ``}`;
    popup.addEventListener('click', e => e.stopPropagation());

    if (offsetX || offsetY) popup.style.transform = `translate(${offsetX}px, ${offsetY}px)`;

    viewer.addOverlay({
      element: popup,
      location: new OpenSeadragon.Point(x, y),
      placement: OpenSeadragon.OverlayPlacement.BOTTOM
    });

    openPopupId = id;

    if (popupTimers.has(id)) clearTimeout(popupTimers.get(id));
    const t = setTimeout(()=>{ closePopup(id); }, 10000);
    popupTimers.set(id, t);
  }

  function closePopup(id){
    const el = document.getElementById(`popup-${id}`);
    if (el) el.remove();
    const dot = document.querySelector(`.hotspot-overlay[data-id="${CSS.escape(id)}"]`);
    if (dot) dot.classList.remove('is-hidden');
    if (popupTimers.has(id)) { clearTimeout(popupTimers.get(id)); popupTimers.delete(id); }
    if (openPopupId === id) openPopupId = null;
  }

  // XML laden
  function loadHotspots(xmlFile) {
    fetch(xmlFile)
      .then(r => r.text())
      .then(str => new window.DOMParser().parseFromString(str, "text/xml"))
      .then(xml => {
        const nodes = xml.getElementsByTagName("HOTSPOT");
        for (let i = 0; i < nodes.length; i++) {
          const node = nodes[i];
          const x = parseFloat(node.getAttribute("X"));
          const y = parseFloat(node.getAttribute("Y"));
          const id = node.getAttribute("ID");

          const iconUrl =
                node.getAttribute("ICON")     ||
                node.getAttribute("ICONURL")  ||
                node.getAttribute("ICON_URL") ||
                node.getAttribute("MARKER")   ||
                node.getAttribute("MEDIA")    ||
                "";

          const popupImage =
                node.getAttribute("POPUP")    ||
                node.getAttribute("POPUPIMG") ||
                node.getAttribute("IMAGE")    ||
                "";

          const popupText  = "";   // nur Bild
          const popupTitle = "";   // nur Bild

          const colorValue =
                node.getAttribute("COLOR")    ||
                node.getAttribute("COLOUR")   ||
                node.getAttribute("FARBE")    ||
                node.getAttribute("FILL")     ||
                node.getAttribute("BG")       ||
                node.getAttribute("DOTCOLOR") ||
                null;

          const offsetX = parseInt(node.getAttribute("POPOFFSETX") || "0", 10);
          const offsetY = parseInt(node.getAttribute("POPOFFSETY") || "0", 10);

          addOverlay(x, y, id, iconUrl || ICON_DEFAULT, popupImage, popupText, popupTitle, colorValue, offsetX, offsetY);
        }
        applyHotspotScale();
      })
      .catch(err => console.error("Error loading XML:", err));
  }
  loadHotspots("./src/hotspots.xml");

  // Helper
  function focusOn(nx, ny, zoomFactor=1.6){
    const ref = new OpenSeadragon.Point(nx, ny);
    viewer.viewport.panTo(ref, true);
    viewer.viewport.zoomBy(zoomFactor, ref, true);
  }

  window.addEventListener('orientationchange', () => setTimeout(applyHotspotScale, 50));
</script>
</body>
</html>
