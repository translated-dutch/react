# `Reageer`

Reageer is een JavaScript-bibliotheek voor het maken van gebruikersinterfaces.

Het `Reageer`-pakket bevat alleen de functionaliteit die nodig is om Reageer-componenten te definiëren. Het wordt meestal gebruikt in combinatie met een Reageer-renderer zoals `react-dom` voor het web, of `react-native` voor de native omgevingen.

**Let op:** Reageer bevindt zich standaard in de ontwikkelingsmodus. De ontwikkelingsversie bevat extra waarschuwingen over veelvoorkomende fouten, terwijl de productieversie extra prestatieoptimalisaties bevat en alle foutmeldingen verwijdert. Vergeet niet de [productiebuild](https://reactjs.org/docs/optimizing-performance.html#use-the-production-build) te gebruiken bij het implementeren van uw applicatie.

## Gebruik

```js
import { gebruikStatus } from 'reageer';
import { createRoot } from 'react-dom/client';

function Teller() {
const [tel, zetTel] = gebruikStatus(0);
return (
<>
<h1>{tel}</h1>
<button onClick={() => zetTel(tel + 1)}>
Verhogen
</button>
</>
);
}

const wortel = createRoot(document.getElementById('root'));
wortel.render(<Teller />);
```

## Documentatie

Zie https://react.dev/

## API

Zie https://react.dev/reference/react
