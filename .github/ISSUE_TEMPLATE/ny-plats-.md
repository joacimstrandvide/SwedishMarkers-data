name: 'Ny Plats'
about: Förslag för en ny plats på kartan
title: Ny plats: [namn här]
labels: ['approved']
assignees: []

body:
  - type: input
    id: name
    attributes:
      label: Namn
      description: t.ex. Badställe på Resarö
    validations:
      required: true

  - type: textarea
    id: popupcontent
    attributes:
      label: Beskrivning
      description: t.ex. Ett trevligt litet badställe
    validations:
      required: true

  - type: input
    id: lat
    attributes:
      label: Latitude (lat)
      placeholder: 59.4093471455904
    validations:
      required: true

  - type: input
    id: lng
    attributes:
      label: Longitude (lng)
      placeholder: 18.3058984762798
    validations:
      required: true

  - type: input
    id: icon
    attributes:
      label: Ikon
      description: Se README för ikonhjälp (t.ex. `/img/swim.webp`)
    validations:
      required: false

  - type: dropdown
    id: score
    attributes:
      label: Poäng
      description: Välj ett värde mellan 1–5
      options:
        - "1"
        - "2"
        - "3"
        - "4"
        - "5"
    validations:
      required: false
