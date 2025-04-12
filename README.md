<!DOCTYPE html>
<html lang="ro">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rase de pisici</title>
    <style>
        body {
            background-color: #ffe6f2;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 20px;
        }

        h1 {
            color: #ff66b2;
            text-align: center;
            font-size: 3em;
            margin-bottom: 30px;
            text-shadow: 1px 1px 2px #fff;
            padding: 10px;
            background-color: #fff;
            border-radius: 8px;
        }

        p {
            max-width: 800px;
            margin: 0 auto 30px;
            font-size: 1.1em;
            line-height: 1.6;
        }

        .cat-card {
            background-color: white;
            border-radius: 15px;
            padding: 20px;
            margin: 20px auto;
            max-width: 800px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s, box-shadow 0.3s, background-color 0.3s;
            cursor: pointer;
        }

        .cat-card:hover {
            transform: translateY(-5px);
            background-color: #fff0f5;
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2);
        }

        .cat-card img {
            width: 100%;
            max-height: 400px;
            object-fit: cover;
            border-radius: 10px;
            margin-bottom: 15px;
            transition: transform 0.3s;
            cursor: pointer;
        }

        .cat-card:hover img {
            transform: scale(1.03);
        }

        h2 {
            color: #cc3399;
            margin-bottom: 10px;
        }

        .more-info {
            display: none;
            margin-top: 10px;
            color: #333;
            font-size: 0.95em;
            background-color: #fce4ec;
            padding: 10px;
            border-radius: 10px;
        }

        button {
            background-color: #ff66b2;
            color: white;
            border: none;
            padding: 10px 15px;
            border-radius: 8px;
            font-size: 1em;
            margin-top: 10px;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        button:hover {
            background-color: #cc3399;
        }

        /* Meniul */
        .menu {
            text-align: center;
            margin-bottom: 20px;
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }

        .menu a {
            background-color: #ff66b2;
            color: white;
            padding: 8px 15px;
            margin: 5px;
            text-decoration: none;
            border-radius: 8px;
            font-size: 1em;
            transition: background-color 0.3s;
        }

        .menu a:hover {
            background-color: #cc3399;
            box-shadow: 0 0 10px rgba(255, 102, 178, 0.7);
        }

        .lightbox {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.8);
            justify-content: center;
            align-items: center;
            z-index: 1000;
        }

        .lightbox img {
            max-width: 90%;
            max-height: 90%;
            object-fit: contain;
        }

        /* Responsivitate */
        @media (max-width: 600px) {
            h1 {
                font-size: 2em;
            }

            p, h2 {
                padding: 0 10px;
            }

            .cat-card {
                margin: 10px;
            }
        }
    </style>
</head>
<body>

    <div class="menu">
        <a href="#persana">Persana</a>
        <a href="#sfinks">Sfinks</a>
        <a href="#mainecoons">Maine Coon</a>
        <a href="#bengaleza">Bengaleza</a>
        <a href="#britishshorthair">British Shorthair</a>
        <a href="#siameza">Siameza</a>
        <a href="#ragdoll">Ragdoll</a>
        <a href="#scottishfold">Scottish Fold</a>
        <a href="#abisiniana">Abisiniana</a>
        <a href="#exoticshorthair">Exotic Shorthair</a>
    </div>

    <h1>Rase de pisici</h1>
    <p>Pisicile sunt animale fascinante, cu o diversitate impresionantă de rase. Unele sunt pufoase și aristocratice, altele energice și jucăușe. Iată zece dintre cele mai cunoscute rase de pisici, fiecare cu farmecul său unic.</p>

    <!-- Pisici -->
    <div class="cat-card" id="persana">
        <img src="https://fera.ro/images/companies/1/BLOG/kot%20perski%203.jpg?1533043631503" alt="Pisica persană" onclick="openLightbox(this)">
        <h2>1. Persana – regina blănii luxoase</h2>
        <p>Temperament: Pisica persană este cunoscută pentru natura sa calmă și afectuoasă. Este o pisică liniștită, care preferă un mediu relaxat și stabil. Se atașează profund de stăpânul său și este ideală pentru persoanele care apreciază compania unei pisici docile și iubitoare.</p>
		<p>Caracteristici: Pisica persană are un corp scund și robust, cu o blană lungă și deasă, care necesită îngrijire regulată. Capul este mare, rotund, cu urechi mici și ochi mari, expresivi. Blana poate veni în diverse culori și modele, iar temperamentul său calm o face potrivită pentru viața de apartament.</p>
        <button onclick="toggleInfo(this)">Află mai mult</button>
        <div class="more-info">Originea pisicii persane datează din secolul al XVII-lea, fiind adusă din Persia (Iranul de azi) în Europa. Este una dintre cele mai vechi și populare rase de pisici.</div>
    </div>

    <div class="cat-card" id="sfinks">
        <img src="https://www.animalepierdute.ro/wp-content/uploads/2019/07/sphynx-pisica-de-rasa.jpg" alt="Pisica Sfinks" onclick="openLightbox(this)">
        <h2>2. Sfinks – frumusețea fără blană</h2>
        <p>Temperament: Pisicile Sfinx sunt afectuoase, prietenoase și foarte sociabile. Se atașează profund de stăpânii lor și sunt adesea descrise ca având un comportament similar cu cel al câinilor, fiind loiale și dornice de atenție.</p>
		<p>Caracteristici: Pisica Sfinx este lipsită de blană, având pielea fină și pliabilă. Are un corp muscular, cu urechi mari și ochi expresivi. Deși nu necesită să fie periată, pielea sa necesită îngrijire regulată pentru a preveni murdăria.</p>
        <button onclick="toggleInfo(this)">Află mai mult</button>
        <div class="more-info">Rasa Sphynx a apărut în anii '60 în Canada, ca rezultat al unei mutații naturale. Lipsa blănii este caracteristica sa definitorie.</div>
    </div>

    <div class="cat-card" id="mainecoons">
        <img src="https://gomagcdn.ro/domains2/petpal.ro/files/files/pisica-maine-coon-220443.jpg" alt="Pisica Maine Coon" onclick="openLightbox(this)">
        <h2>3. Maine Coon – gigantul blând</h2>
        <p>Temperament: Pisicile Maine Coon sunt cunoscute pentru natura lor prietenoasă și sociabilă. Sunt inteligente, jucăușe și se înțeleg bine cu alte animale și copii.</p>
		<p>Caracteristici: Maine Coon este o pisică de talie mare, cu o blană lungă și deasă, adaptată la condițiile climatice reci. Are o coadă lungă și stufoasă, urechi mari și ochi expresivi. Blana necesită îngrijire regulată pentru a preveni încurcarea firelor de păr.</p>
        <button onclick="toggleInfo(this)">Află mai mult</button>
        <div class="more-info">Originea exactă a rasei este necunoscută, dar se crede că Maine Coon a apărut în statul Maine, SUA, fiind o rasă adaptată climatului rece.</div>
    </div>

    <div class="cat-card" id="bengaleza">
        <img src="https://gomagcdn.ro/domains/bonacibo.ro/files/files/pisica-bengaleza-istorie-personalitate-caracteristici-3-4420.png" alt="Pisica Bengaleza" onclick="openLightbox(this)">
        <h2>4. Bengaleza – un tigru în miniatură</h2>
        <p>Temperament: Pisicile Bengaleza sunt active, inteligente și foarte jucăușe. Au un comportament similar cu cel al câinilor, aducând obiecte înapoi la stăpân și adesea jucându-se în apă.</p>
		<p>Caracteristici: Pisica Bengaleza are o blană scurtă, deasă și moale la atingere, cu un model distinctiv de pete. Este o pisică de talie medie, cu un corp atletic și agil. Blana necesită îngrijire minimă, iar pisica este activă și energică.</p>
        <button onclick="toggleInfo(this)">Află mai mult</button>
        <div class="more-info">Rasa a fost creată în anii 1970 prin încrucișarea unei pisici domestice cu o pisică leopard asiatică.</div>
    </div>

    <div class="cat-card" id="britishshorthair">
        <img src="https://cfa.org/wp-content/uploads/2024/04/2023-k07i-BabyrayBlueCheeses.webp" alt="British Shorthair" onclick="openLightbox(this)">
        <h2>5. British Shorthair – aristocrata britanică</h2>
        <p>Temperament: Pisicile British Shorthair sunt calme, rezervate și independente. Sunt loiale și afectuoase cu stăpânii lor, dar apreciază și momentele de singurătate.</p>
		<p>Caracteristici: Pisica British Shorthair are un corp robust, cu o blană scurtă și densă. Ochii sunt mari și rotunzi, iar urechile sunt mici și rotunjite. Blana necesită îngrijire regulată pentru a preveni acumularea de păr mort.</p>
        <button onclick="toggleInfo(this)">Află mai mult</button>
        <div class="more-info">British Shorthair este una dintre cele mai vechi rase britanice, derivată din pisicile aduse de romani în insule.</div>
    </div>

    <div class="cat-card" id="siameza">
        <img src="https://gomagcdn.ro/domains2/petpal.ro/files/files/pisica-siameza-138678.jpg" alt="Pisica Siameză" onclick="openLightbox(this)">
        <h2>6. Siameza – eleganța vocală</h2>
        <p>Temperament: Pisicile Siameze sunt foarte sociabile, comunicative și afectuoase. Au un glas distinctiv și sunt adesea descrise ca având un comportament similar cu cel al câinilor, fiind loiale și dornice de atenție. </p>
		<p>Caracteristici: Pisica Siameză are o blană scurtă, fină și lucioasă, cu un model de culoare specific pe urechi, bot și coadă. Ochii sunt mari și migdalați, de culoare albastră.</p>
        <button onclick="toggleInfo(this)">Află mai mult</button>
        <div class="more-info">Originară din Thailanda (fostul Siam), această rasă a fost foarte apreciată în palatele regale.</div>
    </div>

    <div class="cat-card" id="ragdoll">
        <img src="https://cfa.org/wp-content/uploads/2024/06/2024-c25i-DiamondRagOreo-874x1024.webp" alt="Pisica Ragdoll" onclick="openLightbox(this)">
        <h2>7. Ragdoll – pisica păpușă</h2>
        <p>Numele său provine din tendința de a se relaxa complet atunci când este luată în brațe.</p>
		<p>Temperament: Ragdoll-urile sunt extrem de blânde, afectuoase și sociabile. Se atașează profund de stăpânii lor și se potrivesc bine în familii cu copii sau alte animale. Sunt adesea descrise ca având un comportament de “câine”, urmându-și stăpânii prin casă și dorind să participe la activitățile familiale.</p>
		<p>Caracteristici: Aceste pisici au un corp mare, musculos, și o blană semilungă, deasă, care necesită îngrijire regulată. Ochii lor mari, de un albastru intens, și urechile de dimensiuni medii, cu vârfuri ușor rotunjite, le conferă un aspect distinctiv. Blana lor este de obicei albă, cu extremitățile (urechi, bot, coadă și uneori lăbuțe) de culoare mai închisă, creând un contrast elegant.</p>
        <button onclick="toggleInfo(this)">Află mai mult</button>
        <div class="more-info">Ragdoll a fost dezvoltată în California în anii 1960 și este cunoscută pentru comportamentul calm și docil.</div>
    </div>

    <div class="cat-card" id="scottishfold">
        <img src="https://www.purina.ro/sites/default/files/2021-02/CAT%20HERO_0021_Scottish_fold.jpg" alt="Scottish Fold" onclick="openLightbox(this)">
        <h2>8. Scottish Fold – urechile îndoite</h2>
        <p>Temperament: Pisicile Scottish Fold sunt calme, afectuoase și se adaptează ușor la diferite medii. Sunt prietenoase cu copiii și alte animale, fiind ideale pentru familii. Deși sunt sociabile, ele apreciază și momentele de liniște și independență.</p>
		<p>Caracteristici: Trăsătura definitorie a acestei rase sunt urechile mici, rotunjite, care se pliază spre față, oferindu-le un aspect unic. Au un corp de talie medie, cu o constituție robustă și lăbuțe rotunde. Blana este scurtă până la medie, densă și poate veni în diverse culori și modele.</p>
        <button onclick="toggleInfo(this)">Află mai mult</button>
        <div class="more-info">Rasa a fost descoperită în Scoția în anii '60, de la o pisică cu o mutație naturală a cartilajului urechilor.</div>
    </div>

    <div class="cat-card" id="abisiniana">
        <img src="https://www.zooplus.ro/ghid/wp-content/uploads/2023/11/Pisica-abisiniana.webp" alt="Pisica Abisiniană" onclick="openLightbox(this)">
        <h2>9. Abisiniana – exploratoarea jucăușă</h2>
        <p>Temperament:Pisica abisiniană este liniștită, inteligentă și curioasă. Îi place compania oamenilor și se atașează de familie. Îi plac spațiul și activitatea, este o bună cățărătoare și va aprecia o grădină plină de copaci și locuri înalte. Pisicile abisiniene sunt jucăușe, însă destul de temperate</p>
		<p>Caracteristici:Abisinienele sunt pisici elegante de talie medie, cu corpul suplu și puternic și picioare lungi, subțiri. Au capul rotund, ușor ascuțit spre bot, cu mici smocuri distinctive de păr pe vârful urechilor și ochi mari, migdalați. Blana scurtă și apropiată de corp a unei pisici abisiniene are un aspect distinctiv „cu picățele” datorat benzilor de culori diferite de pe fiecare fir de păr. Cea mai frecventă culoare este roșcat, însă există și alte nuanțe.</p>
        <button onclick="toggleInfo(this)">Află mai mult</button>
        <div class="more-info">Această rasă este considerată una dintre cele mai vechi, cu rădăcini posibil în Egiptul Antic.</div>
    </div>

    <div class="cat-card" id="exoticshorthair">
        <img src="https://www.purina.ro/sites/default/files/styles/ttt_image_510/public/2021-02/CAT%20BREED%20Hero%20Mobile_0028_Exotic_shorthair.jpg?itok=K3VtWflu" alt="Exotic Shorthair" onclick="openLightbox(this)">
        <h2>10. Exotic Shorthair – persana cu păr scurt</h2>
        <p>Temperament:Pisica Exotic Shorthair are același temperament blând și afectuos și nu este la fel de turbulentă ca majoritatea raselor cu păr scurt. Pisicile Exotice sunt foarte fericite dacă le lași singure acasă și dacă au o viață liniștită.</p>
		<p>Caracteristici:Exotic Shorthair este o rasă de pisici de talie medie, scunde și îndesate. Capul este rotund și lat, cu urechi mici depărtate și o față mică. Ochii sunt mari și rotunzi, de culori strălucitoare. Picioarele sunt scurte, groase și puternice, cu labe mari rotunjite și degete acoperite cu ciucuri. Coada este scurtă și stufoasă.</p>
        <button onclick="toggleInfo(this)">Află mai mult</button>
        <div class="more-info">Rasa a fost creată în anii '60 în SUA, prin încrucișarea pisicii persane cu rase cu păr scurt, precum American Shorthair.</div>
    </div>

    <div id="lightbox" class="lightbox" onclick="closeLightbox()">
        <img src="" id="lightbox-image" alt="Lightbox Image">
    </div>

    <script>
        function toggleInfo(button) {
            const info = button.nextElementSibling;
            info.style.display = info.style.display === 'block' ? 'none' : 'block';
        }

        function openLightbox(img) {
            const lightbox = document.getElementById('lightbox');
            const lightboxImage = document.getElementById('lightbox-image');
            lightbox.style.display = 'flex';
            lightboxImage.src = img.src;
        }

        function closeLightbox() {
		            const lightbox = document.getElementById('lightbox');
            lightbox.style.display = 'none';
        }
    </script>

</body>
</html>
