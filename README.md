# vennwalker-53.github.io
Digital Art Portfolio
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#153d68">
<title>Portfolio — Digital Artist</title>
<style>
:root{--navy:#102f50;--blue:#1c5685;--sky:#b9dcf2;--pale:#eaf5fb;--white:#fff;--ink:#101820;--gray:#71808d;--line:rgba(255,255,255,.22)}
*{box-sizing:border-box}html{scroll-behavior:smooth}body{margin:0;background:var(--blue);color:var(--white);font-family:Inter,ui-sans-serif,system-ui,-apple-system,"Segoe UI",sans-serif}
a{color:inherit;text-decoration:none}.wrap{width:min(1120px,calc(100% - 48px));margin:auto}
header{position:sticky;top:0;z-index:5;background:rgba(16,47,80,.92);backdrop-filter:blur(12px);border-bottom:1px solid var(--line)}
.nav{height:76px;display:flex;align-items:center;justify-content:space-between}.brand{font-weight:800;letter-spacing:.12em;font-size:.9rem}.navlinks{display:flex;gap:28px;font-size:.85rem;color:#dcecf7}.navlinks a:hover{color:var(--sky)}
.hero{min-height:590px;display:grid;grid-template-columns:1.15fr .85fr;align-items:center;gap:48px;padding:88px 0 100px;position:relative}
.eyebrow{text-transform:uppercase;letter-spacing:.2em;font-size:.72rem;color:var(--sky);font-weight:700}.hero h1{font-size:clamp(3.5rem,8vw,7.3rem);line-height:.91;letter-spacing:-.075em;margin:22px 0 24px;max-width:760px}.hero h1 span{color:var(--sky);font-family:Georgia,serif;font-weight:400;font-style:italic}.hero p{max-width:470px;color:#d8e7f1;line-height:1.8;font-size:1.02rem}.cta{display:inline-flex;align-items:center;gap:14px;margin-top:22px;background:var(--sky);color:var(--navy);padding:14px 19px;border-radius:3px;font-size:.83rem;font-weight:800}.cta:hover{background:white}
.hero-art{height:390px;position:relative;display:grid;place-items:center}.orb{width:min(330px,80vw);aspect-ratio:1;border-radius:50%;background:linear-gradient(145deg,#dff3ff 0%,#83b9df 48%,#2b6698 100%);position:relative;box-shadow:28px 28px 0 rgba(8,31,54,.24);overflow:hidden}.orb:before{content:"";position:absolute;width:75%;height:75%;border:1px solid rgba(16,47,80,.5);border-radius:50%;left:12%;top:12%;transform:rotate(-35deg) scaleX(.65)}.orb:after{content:"";position:absolute;width:58%;height:130%;background:rgba(255,255,255,.22);transform:rotate(38deg);left:24%;top:-15%;border-radius:50%}.orbit{position:absolute;width:390px;height:160px;border:1px solid rgba(255,255,255,.45);border-radius:50%;transform:rotate(-28deg)}.spark{position:absolute;color:var(--sky);font-size:2rem}.s1{top:25px;right:18px}.s2{bottom:35px;left:10px;font-size:1.2rem}
.section{padding:88px 0;border-top:1px solid var(--line)}.section-head{display:flex;align-items:end;justify-content:space-between;gap:24px;margin-bottom:34px}.section h2{font-size:clamp(2.4rem,5vw,4rem);letter-spacing:-.06em;margin:8px 0 0}.section-intro{color:#d6e6f0;max-width:360px;line-height:1.7;font-size:.92rem}
.projects{display:grid;grid-template-columns:repeat(2,1fr);gap:22px}.project{background:var(--pale);color:var(--ink);border-radius:5px;overflow:hidden}.project:nth-child(2){margin-top:55px}.project:nth-child(4){margin-top:55px}.project-image{height:310px;background:#a8cce3;position:relative;overflow:hidden;display:grid;place-items:center;color:#234b6b}.project-image img{width:100%;height:100%;object-fit:cover;display:block}.placeholder{font-size:.8rem;letter-spacing:.12em;text-transform:uppercase;font-weight:700;text-align:center;padding:20px}.project-body{padding:22px 24px 25px}.project-meta{display:flex;justify-content:space-between;gap:12px;color:#657582;font-size:.7rem;text-transform:uppercase;letter-spacing:.12em}.project h3{font-size:1.55rem;letter-spacing:-.04em;margin:12px 0 8px}.project p{color:#53616c;line-height:1.7;font-size:.9rem;margin:0}
.about-grid{display:grid;grid-template-columns:.8fr 1.2fr;gap:70px;align-items:start}.about-mark{font:italic 4rem Georgia,serif;color:var(--sky);line-height:1}.about-copy{font-size:1.15rem;line-height:1.9;color:#e1edf5;max-width:700px}.about-copy strong{color:white}.contact{background:var(--navy);padding:62px 0;margin-top:20px}.contact-row{display:flex;justify-content:space-between;align-items:center;gap:30px}.contact h2{font-size:clamp(2rem,4vw,3.5rem);letter-spacing:-.06em;margin:0}.contact p{color:#c5d9e8}.contact a{color:var(--sky);border-bottom:1px solid var(--sky);padding-bottom:5px}
footer{padding:25px 0;color:#c0d4e3;font-size:.75rem;display:flex;justify-content:space-between;gap:20px}
.edit-panel{position:fixed;right:18px;bottom:18px;z-index:10;background:#fff;color:#142b3e;padding:13px 15px;border-radius:5px;box-shadow:0 8px 30px #071c3070;display:flex;align-items:center;gap:10px;font-size:.8rem}
.edit-panel button,.upload{border:0;background:var(--navy);color:white;padding:9px 12px;border-radius:3px;font:inherit;font-weight:700;cursor:pointer}.edit-panel button:hover,.upload:hover{background:#27689d}.editor{display:none;background:#dcecf7;color:#102f50;padding:18px;margin-top:10px}.editor.open{display:block}.editor label{display:block;font-size:.75rem;font-weight:800;margin:12px 0 5px}.editor input,.editor textarea{width:100%;border:1px solid #9bb8cc;background:white;padding:9px;font:inherit;color:#102f50}.editor textarea{min-height:75px;resize:vertical}.editor .upload{display:inline-block;margin-top:8px}.editor input[type=file]{display:none}
[contenteditable=true]{outline:2px dashed #8fc4e7;outline-offset:4px}
@media(max-width:760px){.wrap{width:min(100% - 32px,600px)}.nav{height:66px}.navlinks{gap:15px;font-size:.78rem}.hero{grid-template-columns:1fr;padding:65px 0 55px;gap:10px}.hero-art{height:270px}.orb{width:230px}.orbit{width:290px;height:120px}.section{padding:65px 0}.section-head{display:block}.section-intro{margin-top:15px}.projects{grid-template-columns:1fr}.project:nth-child(2),.project:nth-child(4){margin-top:0}.project-image{height:260px}.about-grid{grid-template-columns:1fr;gap:24px}.contact-row{display:block}.contact-row a{display:inline-block;margin-top:15px}footer{display:block}footer span{display:block;margin-top:8px}.edit-panel{right:10px;bottom:10px}}
@media print{header,.edit-panel,.editor{display:none!important}.project{break-inside:avoid}}
</style>
</head>
<body>
<header><div class="wrap nav"><a class="brand" href="#home">YOUR NAME / ART</a><nav class="navlinks"><a href="#work">Work</a><a href="#about">About</a><a href="#contact">Contact</a></nav></div></header>
<main>
<section class="wrap hero" id="home"><div><div class="eyebrow">Digital artist · Portfolio</div><h1>Ideas in<br><span>another</span><br>dimension.</h1><p>A collection of visual experiments, digital worlds, and creative explorations. Welcome to my portfolio.</p><a class="cta" href="#work">EXPLORE THE WORK <span>↘</span></a></div><div class="hero-art"><div class="orbit"></div><div class="orb"></div><div class="spark s1">✳</div><div class="spark s2">✦</div></div></section>
<section class="section" id="work"><div class="wrap"><div class="section-head"><div><div class="eyebrow">Selected work / 01—04</div><h2>Four projects<span style="color:var(--sky)">.</span></h2></div><p class="section-intro">A snapshot of my practice. Each project is a different place to experiment, play, and push an idea further.</p></div>
<div class="projects">
<article class="project"><div class="project-image" id="visual1"><div class="placeholder">Project image 01<br>Upload your artwork below</div></div><div class="project-body"><div class="project-meta"><span>01 / Project</span><span>Year · Medium</span></div><h3 id="title1">Project One</h3><p id="desc1">Add a short description of the concept, process, or story behind this piece.</p><div class="editor" id="editor1"><label>Project title</label><input id="inTitle1" value="Project One"><label>Description</label><textarea id="inDesc1">Add a short description of the concept, process, or story behind this piece.</textarea><label>Artwork image</label><label class="upload" for="file1">Choose image</label><input type="file" id="file1" accept="image/*"></div></div></article>
<article class="project"><div class="project-image" id="visual2"><div class="placeholder">Project image 02<br>Upload your artwork below</div></div><div class="project-body"><div class="project-meta"><span>02 / Project</span><span>Year · Medium</span></div><h3 id="title2">Project Two</h3><p id="desc2">Add a short description of the concept, process, or story behind this piece.</p><div class="editor" id="editor2"><label>Project title</label><input id="inTitle2" value="Project Two"><label>Description</label><textarea id="inDesc2">Add a short description of the concept, process, or story behind this piece.</textarea><label>Artwork image</label><label class="upload" for="file2">Choose image</label><input type="file" id="file2" accept="image/*"></div></div></article>
<article class="project"><div class="project-image" id="visual3"><div class="placeholder">Project image 03<br>Upload your artwork below</div></div><div class="project-body"><div class="project-meta"><span>03 / Project</span><span>Year · Medium</span></div><h3 id="title3">Project Three</h3><p id="desc3">Add a short description of the concept, process, or story behind this piece.</p><div class="editor" id="editor3"><label>Project title</label><input id="inTitle3" value="Project Three"><label>Description</label><textarea id="inDesc3">Add a short description of the concept, process, or story behind this piece.</textarea><label>Artwork image</label><label class="upload" for="file3">Choose image</label><input type="file" id="file3" accept="image/*"></div></div></article>
<article class="project"><div class="project-image" id="visual4"><div class="placeholder">Project image 04<br>Upload your artwork below</div></div><div class="project-body"><div class="project-meta"><span>04 / Project</span><span>Year · Medium</span></div><h3 id="title4">Project Four</h3><p id="desc4">Add a short description of the concept, process, or story behind this piece.</p><div class="editor" id="editor4"><label>Project title</label><input id="inTitle4" value="Project Four"><label>Description</label><textarea id="inDesc4">Add a short description of the concept, process, or story behind this piece.</textarea><label>Artwork image</label><label class="upload" for="file4">Choose image</label><input type="file" id="file4" accept="image/*"></div></div></article>
</div></div></section>
<section class="section" id="about"><div class="wrap about-grid"><div><div class="eyebrow">A little about me</div><div class="about-mark">Hello,</div></div><div class="about-copy" id="aboutText" contenteditable="false">I'm <strong>Your Name</strong>, a digital artist interested in visual storytelling, color, and the space between imagination and reality. My work moves across illustration, image-making, and experimentation. I love building visuals that feel a little unexpected, while keeping the details intentional.</div></div></section>
<section class="contact" id="contact"><div class="wrap contact-row"><div><div class="eyebrow">Have a project in mind?</div><h2>Let's make<br>something good.</h2><p>Get in touch for collaborations, commissions, or just to say hello.</p></div><a href="mailto:hello@example.com" id="emailLink">HELLO@EXAMPLE.COM ↗</a></div></section>
</main>
<footer class="wrap"><div>© <span id="year"></span> YOUR NAME / DIGITAL ARTIST</div><span>Made with curiosity & a little bit of blue.</span></footer>
<div class="edit-panel"><span id="editStatus">Customize your portfolio</span><button id="editBtn">Edit site</button><button id="saveBtn">Save website</button></div>
<script>
document.getElementById('year').textContent=new Date().getFullYear();
let editing=false;
const btn=document.getElementById('editBtn');
btn.addEventListener('click',()=>{
 editing=!editing;btn.textContent=editing?'Finish editing':'Edit site';
 document.getElementById('editStatus').textContent=editing?'Changes are local until you save':'Customize your portfolio';
 document.querySelectorAll('.editor').forEach(e=>e.classList.toggle('open',editing));
 document.getElementById('aboutText').contentEditable=editing?'true':'false';
});
for(let i=1;i<=4;i++){
 const title=document.getElementById('inTitle'+i),desc=document.getElementById('inDesc'+i);
 title.addEventListener('input',()=>document.getElementById('title'+i).textContent=title.value);
 desc.addEventListener('input',()=>document.getElementById('desc'+i).textContent=desc.value);
 document.getElementById('file'+i).addEventListener('change',e=>{
  const f=e.target.files[0];if(!f)return;
  const reader=new FileReader();reader.onload=()=>{document.getElementById('visual'+i).innerHTML='<img alt="Project '+i+' artwork" src="'+reader.result+'">';};reader.readAsDataURL(f);
 });
}
document.getElementById('saveBtn').addEventListener('click',()=>{
 const clone=document.documentElement.cloneNode(true);
 clone.querySelectorAll('.editor').forEach(e=>e.remove());
 clone.querySelectorAll('.edit-panel').forEach(e=>e.remove());
 clone.querySelectorAll('[contenteditable]').forEach(e=>e.removeAttribute('contenteditable'));
 clone.querySelectorAll('script').forEach(e=>e.remove());
 const script=document.createElement('script');
 script.textContent="document.getElementById('year').textContent=new Date().getFullYear();";
 clone.querySelector('body').appendChild(script);
 const blob=new Blob(['<!DOCTYPE html>\\n'+clone.outerHTML],{type:'text/html'});
 const url=URL.createObjectURL(blob),a=document.createElement('a');
 a.href=url;a.download='my-digital-art-portfolio.html';a.click();URL.revokeObjectURL(url);
 document.getElementById('editStatus').textContent='Saved — your updated website downloaded';
});
</script>
</body></html>
