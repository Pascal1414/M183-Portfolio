# A08:2021 – Software- und Datenintegritätsfehler

## Überblick

## Erläuterung zu Aufgabe 3 und 4

CWE – Common Weakness Enumeration. CWE & OWASP Top 10 hängen damit zusammen das OWASP eine Auflistung der häufigsten Sicherheitslücken ist.

## Theoretische Hintergründe

## Schwachstelle mit Codebeispiel

## Massnahmen mit Codebeispiel

Verwenden sie digitale Signaturen, um die Authentizität zu überprüfen.

### Beispiel in Node.js app

```json
"packages":{
    "node_modules/@esbuild/win32-arm64"{
        "version": "0.18.20",
        "resolved": "https://registry.npmjs.org/@esbuild/win32-arm64/-/win32-arm64-0.18.20.tgz",
        "integrity": "sha512-checksum"
    }
}
```

### Beispiel Arch installation

![Arch checksum](src/arch-checksum.png)

Package-lock.json in einer

## Resultate, Erkenntnisse

## Quellen
