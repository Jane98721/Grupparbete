Ska JSON Web Tokens (JWT) användas för auktorisering?
Ja. Fördelar med JWT  är att man kan signera med en privat nyckel vilket skapar mer säkerhet då man kan se om tokenet har manipulerats. 
JWT har även stöd i många programmeringsspråk och ramverk. 

Bör token lagras i local storage, eller ska man använda session-ID och hämta JWT från backend?
Att använda session-ID och hämta JWT från backend är ett mer säkrare alternativ än att lagra i local storage då man kan undvika risken för xxs-attacker. 
Session Id har även en automatisk utgångshantering. Local storage är mer känsligt för xss attacker. 

Ska JWT-lösenordet propageras för att möjliggöra verifiering i varje backend, eller används metoder i auth-servern för autentisering?

Hur ska man hantera token-förnyelse och utgångstider för att upprätthålla säkerheten och användarvänligheten?
Att ha utgångstider är viktigt för säkerheten. En token kan bli stulen och har man en token med kort utgångstid blir det mer säkert då den inte kan användas allt för länge. 
Korta utgångstider minskar även risken för obehörig åtkomst

Vilka säkerhetsmekanismer bör implementeras för att skydda mot Cross-Site Scripting (XSS) och Cross-Site Request Forgery (CSRF)?

Hur implementeras säker lagring och hantering av känslig användarinformation i enlighet med GDPR?
En användare ska kunna begära att deras personuppgifter tas bort ifall de inte längre är nödvändigt att spara dessa. 
Samla endast relevant information. Kryptera informationen. De som har tillgång till den känsliga informationen ska kunna verifiera sin identitet via identifiering och autentisering. 
Vid dataintrång eller andra säkerhetsincidenter ska man ha en tydlig och effektiv plan på hur man ska hantera dessa. 

Vilka strategier bör användas för att säkerställa säker datakommunikation mellan frontend, auth-server och backend?
Använd https och olika autentiseringsmetoder.
Använd post när du skickar känslig data.

Hur balanseras behovet av stark säkerhet med en smidig och användarvänlig inloggningsprocess?

På vilket sätt ska systemet hantera olika användarroller och deras åtkomstnivåer?

Skall  ramverk användas (passport, jwt, ...) eller skall egenutvecklar kod användas
Fördelen med att använda ramverk är att man kan minska risken för sårbarheter då ramverk har genomfört säkerhetsaspekter. 
Utvecklingstiden även minskar eftersom färdiga lösningar finns för de mest vanligaste problemen.

