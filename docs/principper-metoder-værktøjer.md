## Leverancemål og strategisk forankring

I Digitaliseringsteamet leverer vi løsninger der følger kommunens egen, [den fællesoffentlige digitaliseringsstrategi](https://digst.dk/strategier/den-faellesoffentlige-digitaliseringsstrategi/), samt den [fællesoffentlige digitale arkitektur](https://arkitektur.digst.dk/principper-og-regler). Det betyder, at vi arbejder efter en række [principper](https://arkitektur.digst.dk/principper-og-regler) opstillet af Digitaliseringsstyrelsen: 

⚖️ | [Fællesoffentlige principper](https://arkitektur.digst.dk/principper-og-regler) | [Den fællesoffentlige digitaliseringsstrategi](https://digst.dk/strategier/den-faellesoffentlige-digitaliseringsstrategi/) |

## Metoder 

Driftsplatformen bygger på åbne standarder og har fokus på skalering og samarbejde på tværs hvorfor der anvendes ensartede metoder til samarbejde om og styring af udviklingen.
Dette sikrer overholdelse af leverancemålene og den strategiske forankring og samtidigt minimeres risikoen for teknisk gæld.

🔃 | [GitOps](https://www.weave.works/technologies/gitops/) | [Indbygget databeskyttelse (Privacy-as-code)](https://sikkerdigital.dk/myndighed/databeskyttelse-og-gdpr/indbygget-databeskyttelse) | [Docs-as-code](https://www.writethedocs.org/guide/docs-as-code/) | [12Factor App](https://12factor.net/) | [Low-code development](https://architectelevator.com/architecture/low-code-no-code/) | [Polyglot programming](https://www.techtarget.com/searchsoftwarequality/definition/polyglot-programming) |

[Læs mere om hvordan Randers Kommune implementerer Privacy-by-Design her](/docs/privacy-by-design.md)

## Arkitektur

For at kunne leve op til de ovenstående metoder og principper er platformen en levende størrelse i løbende udvikling. Vi bruger et sæt moderne, åbne standardteknologier til at udvikle, udrulle og vedligeholde løsninger.

📐 | [Event driven architecture](https://en.wikipedia.org/wiki/Event-driven_architecture) | [Containerized Architecture](https://www.aquasec.com/cloud-native-academy/container-security/containerized-architecture/) | [Arkitekturoverblik](arkitektur-overblik.md) | 

## Værktøjer og teknologier

Vores digitaliseringsplatform består af en række værktøjer, der hjælper os med at udvikle, implementere og vedligeholde vores digitale løsninger. Herunder er en liste over værktøjer vi anvender til versionskontrol og kodehåndtering, udrulning af løsninger, monitorering, logging og metrics samt identitetskontrol og rollebaseret adgangsstyring. 
Til at levere løsninger der understøtter forvaltningerne arbejder vi derudover med en håndfuld dataformater og forespørgselssprog der kan indsamle og kvalificere data til automatisering, ledelsesinformation og beslutningsstøtte.

#### Versionskontrol og kodehåndtering
🛡️ | [Git](https://git-scm.com/) | [GitHub](https://github.com/) | [GitHub Projects](https://docs.github.com/en/repositories/organizing-your-repository-with-projects/about-project-boards) | [GitHub Codespaces](https://github.com/features/codespaces) |

#### Containerisering
📦 | [Docker-containere](https://www.docker.com/resources/what-container) | [Kubernetes](https://kubernetes.io/) | [Helm](https://helm.sh/)

#### Identitetskontrol og rollebaseret adgangsstyring
🔑 | [Keycloak](https://www.keycloak.org/) |

#### Monitorering, Logging og metrics
📉 | [Prometheus](https://prometheus.io/) | [Grafana](https://grafana.com/oss/) |

#### Server-side teknologier
⚙️ | [Python](https://www.python.org/) | [JavaScript](https://developer.mozilla.org/da/docs/Web/JavaScript) | [Node.js](https://nodejs.org/) | [Node-RED](https://nodered.org/) |

#### Klient-side teknologier
🖥️ | [VueJS](https://vuejs.org/) |

#### Datatræk
🔀 | [REST](https://restfulapi.net/) | [SOAP](https://www.w3.org/TR/soap/) | [SFTP](https://en.wikipedia.org/wiki/SSH_File_Transfer_Protocol) | [Puppeteer](https://pptr.dev/) | [Browserless](https://www.browserless.io/) |

####  Dataformatering og forespørgselssprog
🗃️ | [JSON](https://www.json.org/json-da.html) | [JSONata](https://jsonata.org/) | [SQL](https://en.wikipedia.org/wiki/SQL) |

#### Data Visualisering og Analytics
📊 | [Apache Superset](https://superset.apache.org/) |

## Teknologier under afprøvning

Vi er altid på udkig efter nye teknologier og afprøver dem i vores udviklingslaboratorium.

🧪 | [Udviklingslaboratoriet](udviklingslaboratorie.md) |
