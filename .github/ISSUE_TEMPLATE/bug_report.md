name: 🐛 Bug Report
description: Einen Fehler melden
labels: ["type:bug", "priority:normal"]
body:
  - type: markdown
    attributes:
      value: "Danke für den Bug Report. Bitte fülle alle Felder aus."

  - type: textarea
    id: description
    attributes:
      label: Beschreibung
      description: Was ist passiert? Was hast du erwartet?
    validations:
      required: true

  - type: textarea
    id: steps
    attributes:
      label: Schritte zum Reproduzieren
      placeholder: "1. ...\n2. ...\n3. ..."
    validations:
      required: true

  - type: dropdown
    id: severity
    attributes:
      label: Schweregrad
      options: [Critical, High, Normal, Low]
    validations:
      required: true
