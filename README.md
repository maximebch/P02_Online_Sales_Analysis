# P02_Online_Sales_Analysis
<h2><strong><em>Data Analyst Certification by OpenClassrooms, in partnership with&nbsp;ENSAE-ENSAI</em></strong></h2>
<div>
    <div>
        <div>
            <div>
                <div>
                    <div>
                        <div>
                            <div>
                                <p><em>Analyzing e-commerce sales using Python</em></p>
                                <p><em>Skills:</em></p>
                                <ul>
                                    <li><em>Describe a dataset using descriptive statistics</em></li>
                                    <li><em>Master basic statistical concepts</em></li>
                                    <li><em>Clean a dataset</em></li>
                                </ul>
                                <p><em><br></em></p>
                                <h1>Analysez les ventes de votre entreprise</h1>
                            </div>
                        </div>
                    </div>
                    <div><br></div>
                </div>
                <div>
                    <h3>Pr&eacute;requis</h3>
                    <p>Les pr&eacute;requis pour ce projet sont de conna&icirc;tre au choix les langages <strong>R</strong> ou <strong>Python</strong>, en sachant manipuler principalement les <em>Dataframes&nbsp;</em>(natifs en R, ou disponibles par la librairie Pandas en Python). Il vous faudra &eacute;galement conna&icirc;tre les bases de la statistique descriptive (moyenne, m&eacute;diane, variance, repr&eacute;sentations graphiques, tests de corr&eacute;lation, analyse bivari&eacute;e, etc.).</p>
                    <p>&nbsp;</p>
                    <h3>Sc&eacute;nario</h3>
                    <p>Vous &ecirc;tes data analyst d&apos;une grande cha&icirc;ne de librairie, fra&icirc;chement embauch&eacute; depuis une semaine ! Vous avez fait connaissance avec vos coll&egrave;gues, votre nouveau bureau, mais surtout, la machine &agrave; caf&eacute; high-tech : Rien que &ccedil;a !</p>
                    <p>Mais revenons &agrave; votre mission : il est temps de mettre les mains dans le cambouis ! Le service Informatique vous a donn&eacute; l&rsquo;acc&egrave;s &agrave; la base de donn&eacute;es des ventes. &Agrave; vous de vous familiariser avec les donn&eacute;es, et de les analyser. Votre manager souhaite que vous r&eacute;alisiez une pr&eacute;sentation pour vous &quot;faire la main&quot;.</p>
                    <p>Comme vous l&apos;avez appris dans vos recherches avant de postuler, votre entreprise, &quot;Rester livres&quot; s&apos;est d&apos;abord d&eacute;velopp&eacute;e dans une grande ville de France, avec plusieurs magasins, jusqu&apos;&agrave; d&eacute;cider d&apos;ouvrir une boutique en ligne. Son&nbsp;approche de la vente de livres en ligne, bas&eacute;e sur des algorithmes de recommandation, lui&nbsp;a valu un franc succ&egrave;s !</p>
                    <h3>Les donn&eacute;es</h3>
                    <p>Vous avez acc&egrave;s &agrave; ces donn&eacute;es, extraites directement de la base de l&rsquo;entreprise vers les fichiers CSV. Voici les fichiers &agrave; votre disposition :</p>
                    <ul>
                        <li>les ventes (appel&eacute;es &ldquo;Transactions&rdquo;) ;</li>
                        <li>la liste des clients ;</li>
                        <li>la liste des produits.</li>
                    </ul>
                    <aside>
                        <p>T&eacute;l&eacute;chargez le jeu de donn&eacute;es &agrave; <a href="https://s3-eu-west-1.amazonaws.com/static.oc-static.com/prod/courses/files/parcours-data-analyst/dataset_P4.zip">cette adresse</a>.</p>
                    </aside>
                    <h3>Vos missions</h3>
                    <h4>Mission n&deg; 1</h4>
                    <p>Avant de pouvoir entrer dans le vif du sujet, il vous faudra faire un peu de nettoyage ! Par exemple, vous devrez faire des choix quant au traitement des valeurs manquantes et des valeurs aberrantes.</p>
                    <h4>Mission n&deg; 2</h4>
                    <p>Ensuite, vous r&eacute;aliserez l&rsquo;analyse des donn&eacute;es. Une grande libert&eacute; vous est laiss&eacute;e sur ce plan, mais &agrave; vous de trouver les informations qui ont du sens pour mieux comprendre les ventes.</p>
                    <p>Vous devrez y utiliser au moins :</p>
                    <ul>
                        <li>des indicateurs de tendance centrale et de dispersion ;</li>
                        <li>une analyse de concentration, via une courbe de Lorenz et un indice de Gini ;</li>
                        <li>des repr&eacute;sentations graphiques, dont au moins un histogramme, une repr&eacute;sentation avec des &quot;bo&icirc;tes &agrave; moustaches&quot;, et une repr&eacute;sentation de s&eacute;rie temporelle (c&rsquo;est-&agrave;-dire un graphique dont l&rsquo;axe des abscisses repr&eacute;sente des dates) ;</li>
                        <li>des analyses bivari&eacute;es.</li>
                    </ul>
                    <h4>Mission n&deg; 3</h4>
                    <p>Voici quelques questions&nbsp;suppl&eacute;mentaires, que votre manager vous a pos&eacute;es :</p>
                    <ol>
                        <li>Y a-t-il une corr&eacute;lation entre le sexe des clients et les cat&eacute;gories de produits achet&eacute;s ?</li>
                        <li>Y a-t-il une corr&eacute;lation entre l&apos;&acirc;ge des clients et :<ul>
                                <li>Le montant total des achats ;</li>
                                <li>La fr&eacute;quence d&rsquo;achat (ie. nombre d&apos;achats par mois par exemple) ;</li>
                                <li>La taille du panier moyen (en nombre d&rsquo;articles) ;</li>
                                <li>Les cat&eacute;gories de produits achet&eacute;s.</li>
                            </ul>
                        </li>
                    </ol>
                    <aside>
                        <p>Pour les corr&eacute;lations, pas besoin d&apos;effectuer en entier les tests (chi-2, ANOVA, etc.). Seul le calcul des statistiques de test est demand&eacute; (\(r^2, \eta^2, \xi_n\)).</p>
                    </aside>
                    <aside>
                        <h5>Quelques pr&eacute;cisions</h5>
                        <ul>
                            <li>Vous avez le choix entre 2 langages : R ou Python. Dans les deux cas, vos donn&eacute;s devront &ecirc;tre manipul&eacute;es via les structures Dataframe ou Matrice (pr&eacute;sentes nativement sous R, ou dans la librairie Pandas sous Python).</li>
                            <li>Pour plus de simplicit&eacute;, nous consid&eacute;rons ici que les prix des articles ne varient pas en fonction du temps.</li>
                        </ul>
                    </aside>
                    <h3>Livrables</h3>
                    <p>Un fichier .zip contenant ces fichiers :</p>
                    <ul>
                        <li>le <strong>script</strong> destin&eacute; &agrave; nettoyer le jeu de donn&eacute;es ;</li>
                        <li>le <strong>script</strong> contenant les diff&eacute;rentes analyses effectu&eacute;es ;</li>
                        <li>les <strong>graphiques</strong> dans un format image (PNG ou JPG) ;</li>
                        <li>un court <strong>fichier README</strong>, contenant les explications pour lancer vos scripts.</li>
                    </ul>
                    <aside>
                        <p>Pour faciliter votre passage au jury, d&eacute;posez sur la plateforme, dans un dossier nomm&eacute; &ldquo;<em>P4_nom_prenom</em>&rdquo;, tous les livrables du projet. Chaque livrable doit &ecirc;tre nomm&eacute; avec le num&eacute;ro du projet et selon l&apos;ordre dans lequel il appara&icirc;t, par exemple &ldquo;<em>P4_01_scriptdonn&eacute;es</em>&rdquo;, &ldquo;<em>P4_02_scriptanalyse</em>&rdquo;, et ainsi de suite.</p>
                    </aside>
                    <h3>Soutenance</h3>
                    <aside>
                        <p>Vous serez amen&eacute; &agrave; cr&eacute;er des graphiques. Il y a certains pi&egrave;ges dans lesquels il ne faut pas tomber : veillez bien &agrave; respecter les r&egrave;gles donn&eacute;es dans <a href="https://openclassrooms.com/fr/courses/4525336-realisez-des-rapports-statistiques-clairs-et-impactants/5312796-evitez-les-pieges-des-graphiques">ce chapitre</a>. Pensez &eacute;galement &agrave; votre examinateur : si votre pr&eacute;sentation n&apos;est pas donn&eacute;e en plein &eacute;cran, et si l&apos;&eacute;cran de votre examinateur est plus petit que le v&ocirc;tre, il risque de ne pas pouvoir lire correctement les graphiques, les l&eacute;gendes ou les noms des axes.</p>
                    </aside>
                    <p>La soutenance, d&apos;une dur&eacute;e de 30 minutes, &nbsp;se d&eacute;roule en 3 &eacute;tapes :</p>
                    <ol>
                        <li>D&eacute;tail du nettoyage des donn&eacute;es : quelles valeurs aberrantes et manquantes avez-vous trouv&eacute;es, comment les avez-vous trait&eacute;es, avez-vous effectu&eacute; d&apos;autres nettoyages ? (10 minutes)</li>
                        <li>Pr&eacute;sentation de l&apos;analyse demand&eacute;e, &agrave; l&apos;aide d&apos;un logiciel de pr&eacute;sentation adapt&eacute;. (10 minutes)</li>
                        <li>Pr&eacute;sentez votre analyse des corr&eacute;lations, en les interpr&eacute;tant. (10 minutes)</li>
                        <li>S&eacute;ance de questions-r&eacute;ponses &eacute;ventuelle.&nbsp;</li>
                    </ol>
                </div>
                <h3>Comp&eacute;tences &eacute;valu&eacute;es</h3>
                <ul>
                    <li>
                        <div>
                            <div><svg width="20" height="20" xmlns="http://www.w3.org/2000/svg" fill="currentColor">
                                    <path d="M11.8023 15.6775V16.1276C11.8023 16.4812 11.5276 16.777 11.1724 16.822L11.0584 17.2271C10.9914 17.4457 10.7837 17.6 10.5558 17.6H9.43664C9.19538 17.6 8.98763 17.4457 8.93401 17.2271L8.82009 16.822C8.4649 16.777 8.19013 16.4812 8.19013 16.1276V15.6775C8.19013 15.446 8.38448 15.2467 8.63914 15.2467H11.3667C11.6147 15.2596 11.8023 15.446 11.8023 15.6775ZM13.8999 9.69139C13.8999 10.6944 13.4777 11.6268 12.8009 12.289C12.2848 12.797 11.9431 13.4528 11.8358 14.1601C11.7889 14.4559 11.5141 14.6873 11.1925 14.6873H8.77317C8.45149 14.6873 8.17673 14.4687 8.12981 14.1601C8.01589 13.4657 7.6808 12.797 7.16478 12.289C6.50131 11.6203 6.08581 10.7266 6.06571 9.7364C6.0523 7.64673 7.77463 5.96212 9.93926 5.94283C12.1441 5.92997 13.8999 7.61458 13.8999 9.69139ZM10.4352 7.42811C10.4352 7.19664 10.2408 7.01018 9.99958 7.01018C8.45149 7.01018 7.17818 8.21898 7.17818 9.71711C7.17818 9.94859 7.37253 10.1351 7.61379 10.1351C7.85505 10.1351 8.0494 9.94859 8.0494 9.71711C8.0494 8.69478 8.92061 7.85891 9.98617 7.85891C10.2408 7.84605 10.4352 7.65958 10.4352 7.42811ZM9.99958 4.72117C10.2408 4.72117 10.4352 4.53471 10.4352 4.30324V2.81796C10.4352 2.58649 10.2408 2.40002 9.99958 2.40002C9.75832 2.40002 9.56397 2.58649 9.56397 2.81796V4.30324C9.56397 4.53471 9.75832 4.72117 9.99958 4.72117ZM4.8192 9.69139C4.8192 9.45992 4.62485 9.27346 4.38359 9.27346H2.83551C2.59425 9.27346 2.3999 9.45992 2.3999 9.69139C2.3999 9.92287 2.59425 10.1093 2.83551 10.1093H4.38359C4.61145 10.1093 4.8192 9.92287 4.8192 9.69139ZM17.1636 9.27346H15.6156C15.3743 9.27346 15.18 9.45992 15.18 9.69139C15.18 9.92287 15.3743 10.1093 15.6156 10.1093H17.1636C17.4049 10.1093 17.5992 9.92287 17.5992 9.69139C17.6127 9.45992 17.4183 9.27346 17.1636 9.27346ZM5.70382 13.2021L4.61145 14.2565C4.4372 14.4237 4.4372 14.6873 4.61145 14.8609C4.69187 14.9381 4.8058 14.9831 4.91972 14.9831C5.03365 14.9831 5.14758 14.9381 5.228 14.8609L6.32707 13.8065C6.50131 13.6393 6.50131 13.3757 6.32707 13.2021C6.15953 13.0477 5.88476 13.0477 5.70382 13.2021ZM13.9804 6.3029C14.0943 6.3029 14.2082 6.25789 14.2886 6.18074L15.3877 5.12625C15.5619 4.95908 15.5619 4.69546 15.3877 4.52185C15.2135 4.34825 14.9387 4.35468 14.7577 4.52185L13.6587 5.56991C13.4844 5.73708 13.4844 6.0007 13.6587 6.17431C13.7592 6.25146 13.8731 6.3029 13.9804 6.3029ZM5.70382 6.17431C5.78424 6.25146 5.89816 6.29647 6.01209 6.29647C6.12602 6.29647 6.23995 6.25146 6.32037 6.17431C6.49461 6.00713 6.49461 5.74351 6.32037 5.56991L5.2213 4.52185C5.04706 4.35468 4.77229 4.35468 4.59134 4.52185C4.4104 4.68903 4.4171 4.95265 4.59134 5.12625L5.70382 6.17431ZM14.2886 13.2021C14.1144 13.0349 13.8396 13.0349 13.6587 13.2021C13.4777 13.3692 13.4844 13.6329 13.6587 13.8065L14.7577 14.8609C14.8382 14.9381 14.9521 14.9831 15.066 14.9831C15.18 14.9831 15.2939 14.9381 15.3743 14.8609C15.5485 14.6938 15.5485 14.4301 15.3743 14.2565L14.2886 13.2021Z"></path>
                                </svg></div>
                        </div>
                        <div>D&eacute;crire un jeu de donn&eacute;es par la statistique descriptive</div>
                    </li>
                    <li>
                        <div>
                            <div><svg width="20" height="20" xmlns="http://www.w3.org/2000/svg" fill="currentColor">
                                    <path d="M11.8023 15.6775V16.1276C11.8023 16.4812 11.5276 16.777 11.1724 16.822L11.0584 17.2271C10.9914 17.4457 10.7837 17.6 10.5558 17.6H9.43664C9.19538 17.6 8.98763 17.4457 8.93401 17.2271L8.82009 16.822C8.4649 16.777 8.19013 16.4812 8.19013 16.1276V15.6775C8.19013 15.446 8.38448 15.2467 8.63914 15.2467H11.3667C11.6147 15.2596 11.8023 15.446 11.8023 15.6775ZM13.8999 9.69139C13.8999 10.6944 13.4777 11.6268 12.8009 12.289C12.2848 12.797 11.9431 13.4528 11.8358 14.1601C11.7889 14.4559 11.5141 14.6873 11.1925 14.6873H8.77317C8.45149 14.6873 8.17673 14.4687 8.12981 14.1601C8.01589 13.4657 7.6808 12.797 7.16478 12.289C6.50131 11.6203 6.08581 10.7266 6.06571 9.7364C6.0523 7.64673 7.77463 5.96212 9.93926 5.94283C12.1441 5.92997 13.8999 7.61458 13.8999 9.69139ZM10.4352 7.42811C10.4352 7.19664 10.2408 7.01018 9.99958 7.01018C8.45149 7.01018 7.17818 8.21898 7.17818 9.71711C7.17818 9.94859 7.37253 10.1351 7.61379 10.1351C7.85505 10.1351 8.0494 9.94859 8.0494 9.71711C8.0494 8.69478 8.92061 7.85891 9.98617 7.85891C10.2408 7.84605 10.4352 7.65958 10.4352 7.42811ZM9.99958 4.72117C10.2408 4.72117 10.4352 4.53471 10.4352 4.30324V2.81796C10.4352 2.58649 10.2408 2.40002 9.99958 2.40002C9.75832 2.40002 9.56397 2.58649 9.56397 2.81796V4.30324C9.56397 4.53471 9.75832 4.72117 9.99958 4.72117ZM4.8192 9.69139C4.8192 9.45992 4.62485 9.27346 4.38359 9.27346H2.83551C2.59425 9.27346 2.3999 9.45992 2.3999 9.69139C2.3999 9.92287 2.59425 10.1093 2.83551 10.1093H4.38359C4.61145 10.1093 4.8192 9.92287 4.8192 9.69139ZM17.1636 9.27346H15.6156C15.3743 9.27346 15.18 9.45992 15.18 9.69139C15.18 9.92287 15.3743 10.1093 15.6156 10.1093H17.1636C17.4049 10.1093 17.5992 9.92287 17.5992 9.69139C17.6127 9.45992 17.4183 9.27346 17.1636 9.27346ZM5.70382 13.2021L4.61145 14.2565C4.4372 14.4237 4.4372 14.6873 4.61145 14.8609C4.69187 14.9381 4.8058 14.9831 4.91972 14.9831C5.03365 14.9831 5.14758 14.9381 5.228 14.8609L6.32707 13.8065C6.50131 13.6393 6.50131 13.3757 6.32707 13.2021C6.15953 13.0477 5.88476 13.0477 5.70382 13.2021ZM13.9804 6.3029C14.0943 6.3029 14.2082 6.25789 14.2886 6.18074L15.3877 5.12625C15.5619 4.95908 15.5619 4.69546 15.3877 4.52185C15.2135 4.34825 14.9387 4.35468 14.7577 4.52185L13.6587 5.56991C13.4844 5.73708 13.4844 6.0007 13.6587 6.17431C13.7592 6.25146 13.8731 6.3029 13.9804 6.3029ZM5.70382 6.17431C5.78424 6.25146 5.89816 6.29647 6.01209 6.29647C6.12602 6.29647 6.23995 6.25146 6.32037 6.17431C6.49461 6.00713 6.49461 5.74351 6.32037 5.56991L5.2213 4.52185C5.04706 4.35468 4.77229 4.35468 4.59134 4.52185C4.4104 4.68903 4.4171 4.95265 4.59134 5.12625L5.70382 6.17431ZM14.2886 13.2021C14.1144 13.0349 13.8396 13.0349 13.6587 13.2021C13.4777 13.3692 13.4844 13.6329 13.6587 13.8065L14.7577 14.8609C14.8382 14.9381 14.9521 14.9831 15.066 14.9831C15.18 14.9831 15.2939 14.9381 15.3743 14.8609C15.5485 14.6938 15.5485 14.4301 15.3743 14.2565L14.2886 13.2021Z"></path>
                                </svg></div>
                        </div>
                        <div>Ma&icirc;triser les concepts statistiques fondamentaux</div>
                    </li>
                    <li>
                        <div>
                            <div><svg width="20" height="20" xmlns="http://www.w3.org/2000/svg" fill="currentColor">
                                    <path d="M11.8023 15.6775V16.1276C11.8023 16.4812 11.5276 16.777 11.1724 16.822L11.0584 17.2271C10.9914 17.4457 10.7837 17.6 10.5558 17.6H9.43664C9.19538 17.6 8.98763 17.4457 8.93401 17.2271L8.82009 16.822C8.4649 16.777 8.19013 16.4812 8.19013 16.1276V15.6775C8.19013 15.446 8.38448 15.2467 8.63914 15.2467H11.3667C11.6147 15.2596 11.8023 15.446 11.8023 15.6775ZM13.8999 9.69139C13.8999 10.6944 13.4777 11.6268 12.8009 12.289C12.2848 12.797 11.9431 13.4528 11.8358 14.1601C11.7889 14.4559 11.5141 14.6873 11.1925 14.6873H8.77317C8.45149 14.6873 8.17673 14.4687 8.12981 14.1601C8.01589 13.4657 7.6808 12.797 7.16478 12.289C6.50131 11.6203 6.08581 10.7266 6.06571 9.7364C6.0523 7.64673 7.77463 5.96212 9.93926 5.94283C12.1441 5.92997 13.8999 7.61458 13.8999 9.69139ZM10.4352 7.42811C10.4352 7.19664 10.2408 7.01018 9.99958 7.01018C8.45149 7.01018 7.17818 8.21898 7.17818 9.71711C7.17818 9.94859 7.37253 10.1351 7.61379 10.1351C7.85505 10.1351 8.0494 9.94859 8.0494 9.71711C8.0494 8.69478 8.92061 7.85891 9.98617 7.85891C10.2408 7.84605 10.4352 7.65958 10.4352 7.42811ZM9.99958 4.72117C10.2408 4.72117 10.4352 4.53471 10.4352 4.30324V2.81796C10.4352 2.58649 10.2408 2.40002 9.99958 2.40002C9.75832 2.40002 9.56397 2.58649 9.56397 2.81796V4.30324C9.56397 4.53471 9.75832 4.72117 9.99958 4.72117ZM4.8192 9.69139C4.8192 9.45992 4.62485 9.27346 4.38359 9.27346H2.83551C2.59425 9.27346 2.3999 9.45992 2.3999 9.69139C2.3999 9.92287 2.59425 10.1093 2.83551 10.1093H4.38359C4.61145 10.1093 4.8192 9.92287 4.8192 9.69139ZM17.1636 9.27346H15.6156C15.3743 9.27346 15.18 9.45992 15.18 9.69139C15.18 9.92287 15.3743 10.1093 15.6156 10.1093H17.1636C17.4049 10.1093 17.5992 9.92287 17.5992 9.69139C17.6127 9.45992 17.4183 9.27346 17.1636 9.27346ZM5.70382 13.2021L4.61145 14.2565C4.4372 14.4237 4.4372 14.6873 4.61145 14.8609C4.69187 14.9381 4.8058 14.9831 4.91972 14.9831C5.03365 14.9831 5.14758 14.9381 5.228 14.8609L6.32707 13.8065C6.50131 13.6393 6.50131 13.3757 6.32707 13.2021C6.15953 13.0477 5.88476 13.0477 5.70382 13.2021ZM13.9804 6.3029C14.0943 6.3029 14.2082 6.25789 14.2886 6.18074L15.3877 5.12625C15.5619 4.95908 15.5619 4.69546 15.3877 4.52185C15.2135 4.34825 14.9387 4.35468 14.7577 4.52185L13.6587 5.56991C13.4844 5.73708 13.4844 6.0007 13.6587 6.17431C13.7592 6.25146 13.8731 6.3029 13.9804 6.3029ZM5.70382 6.17431C5.78424 6.25146 5.89816 6.29647 6.01209 6.29647C6.12602 6.29647 6.23995 6.25146 6.32037 6.17431C6.49461 6.00713 6.49461 5.74351 6.32037 5.56991L5.2213 4.52185C5.04706 4.35468 4.77229 4.35468 4.59134 4.52185C4.4104 4.68903 4.4171 4.95265 4.59134 5.12625L5.70382 6.17431ZM14.2886 13.2021C14.1144 13.0349 13.8396 13.0349 13.6587 13.2021C13.4777 13.3692 13.4844 13.6329 13.6587 13.8065L14.7577 14.8609C14.8382 14.9381 14.9521 14.9831 15.066 14.9831C15.18 14.9831 15.2939 14.9381 15.3743 14.8609C15.5485 14.6938 15.5485 14.4301 15.3743 14.2565L14.2886 13.2021Z"></path>
                                </svg></div>
                        </div>
                        <div>Nettoyer un jeu de donn&eacute;es</div>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</div>
