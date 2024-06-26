---
title: Wstęp
description: Wstęp do stacka T3
layout: ../../layouts/docs.astro
lang: pl
---

<div class="embed">
<iframe width="560" height="315" src="https://www.youtube.com/embed/d5x0JCZbAJs" title="The best stack for your next project" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

## T3 Stack

_"T3 Stack"_, to stack do web developmentu stworzony przez [Theo](https://twitter.com/t3dotgg) i mający na celu prostotę, modularność oraz typesafety całego projektu.

Jego głównymi elementami są [**Next.js**](https://nextjs.org/) oraz [**TypeScript**](https://typescriptlang.org/). [**Tailwind CSS**](https://tailwindcss.com/) również jest prawie zawsze dołączony. Jeżeli budujesz cokolwiek wspólnego z backendem, [**tRPC**](https://trpc.io/), [**Prisma**](https://prisma.io/) oraz [**NextAuth.js**](https://next-auth.js.org/) mogą być dobrymi dodatkami.

Mogłeś dostrzec już, iż jest tu... dużo elementów. Jest to celowe. Zmieniaj elementy jak tylko chcesz - stack ten jest tak modularny, jak to tylko możliwe.

## A więc... co to Create T3 App? Jakiś szablon?

Może? Create T3 App to narzędzie CLI zbudowane przez doświadczonych deweloperów stacka T3 aby usprawnić zakładanie w nim nowych, modularnych projektów. Oznacza to, iż każdy element jest opcjonalny a "szablon" generowany jest bazując na twoich szczegółowych potrzebach.

Po niezliczonych projektach i wielu latach w tej technologii, nabyliśmy wiele opinii i wewnętrznych doświadczeń. Zrobiliśmy, co tylko się dało, aby zawrzeć je w naszym CLI.

**NIE** jest to szablon all-inclusive. **Oczekujemy** od Ciebie trochę wkładu, dodając biblioteki rozwiązujące problemy, które posiada **TWOJA** aplikacja. Nie chcemy zapisywać rozwiązań na bardziej specyficzne problemy, takie jak state management lub deployment. [Mamy jednak tutaj parę rekomendacji](/pl/other-recs).

## Aksjomaty T3

Będziemy z tobą szczerzy - jest to _kontrowersyjny_ projekt. Posiadamy garść założeń dotyczących budowania aplikacji i traktujemy je jako bazę naszych decyzji.

### Rozwiązuj Problemy

Łatwo jest wpaść w pułapkę "dodawania wszystkiego" - wyraźnie nie chcemy tego robić. Wszystko dodane do Create T3 App powinno rozwiązywać konkretny problem który istnieje w dołączonych technologiach. Znaczy to, że nie dodamy rzeczy, takich jak biblioteki do state managementu (`zustand`, `redux`) ale dodamy elementy takie jak NextAuth.js, Prisma i tRPC.

### "Bleed Responsibly" (Korzystaj Rozważnie z Nowych Technologii)

Kochamy technologie "bleeding edge". Uzyskana prędkość oraz szczerze mówiąc, zabawa, jaka wynika z ich zastosowania - jest naprawdę super. Uważamy jednak za ważne odpowiedzialne korzystanie z powyższych elementów. Oznacza to, iż nie ⛔️ postawimy na nowy rodzaj bazy danych (SQL jest dobry!). Z radością ✅ stawiamy jednak na tRPC - są to tylko funkcje, które łatwo można zamienić na coś innego.

### Typesafety NIE Jest Opcjonalne

Celem Create T3 App jest zapewnienie jak najszybszego sposobu na stworzenie nowego projektu full-stack z pełnym **typesafety**. Typesafety traktujemy poważnie - pozwala ono poprawić naszą produktywność i pomaga nam w dostarczaniu mniejszej ilości bugów. Jakakolwiek decyzja, która naraża naturę typesafety jest decyzją, która powinna zostać podjęta w innym projekcie.
