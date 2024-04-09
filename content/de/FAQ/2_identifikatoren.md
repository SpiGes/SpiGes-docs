---
title: Identifikatoren 
slug: identifikatoren
description: " "
weight: 20
type: docs
keywords: []
---

{{<alert color="info">}}
Die Dokumentation befindet sich im Aufbau.
{{</alert>}}

{{<collapsible title="Die AHVN ist ein Pflichtfeld. Trotzdem wird es Fälle ohne AHV-Nr. geben. Wo ist beschrieben was in diesem Fall in die Variable kommt?">}}
Genau diese Frage ist noch offen. Im Datensatz steht: «Anmerkung: Bezüglich der Personen, die keine AHV-Nummer haben können, sind noch Abklärungen im Gange (vgl. auch Spalte "Anzugeben für").» Kurzfristig ist angedacht, die Variable in diesem Falle leer zu lassen resp. eine Dummy-Nummer anzugeben. Es gab nun aber starken Widerstand dagegen aus einigen Grenzkantonen, weshalb diese Frage langfristig noch genauer abgeklärt wird.
{{</collapsible>}}

{{<collapsible title="Bei der Datenerhebung soll ja die AHVN genutzt werden. Wird die AHVN über die Tarifpartner auch an die Krankenkassen ersichtlich sein werden?">}}
Bei der Datenübermittlung werden Identifikatoren und Daten separat verschickt. Der Datenkanal ist verschlüsselt. Zur Überprüfung der AHVN wird der «BFS AHVN Validator» eingesetzt. Nachdem die AHVN verschlüsselt worden ist, wird diese auf der gesicherten Identifikatoren Datenbank gespeichert. Während der Bearbeitung der Daten auf der Plattform ist die AHVN somit pseudonymisiert und nicht zusammen mit dem Leistungsdatensatz abgelegt. Die AHVN kann nur verschlüsselt an die Datennut-zer weitergegeben werden. Da diese Datennutzer den Schlüssel nicht kennen, ist für diese die AHVN anonymisiert. Ein Rückschluss auf den Originalwert ist nicht möglich.
{{</collapsible>}}

{{<collapsible title="Hat der Kanton Zugang zum ID-File der Lieferungen?">}}
Der Kanton kann während der Erhebung zu Plausibilisierungszwecken Daten exportieren, dabei wird die AHVN pseudonymisiert werden.
{{</collapsible>}}