# page.home

                                        [id]: homepage_v1
                                        [type]: page_spec
                                        [version]: 1

                                        ## meta
                                        title: "Arjun Phlox"
                                        route: "/"
                                        language: "en-IN"

                                        ## layout
                                        sections:
                                          - id: hero_v1
                                              slot: "hero"
                                                  component: "Hero"
                                                      source: "./hero.skill.md"
                                                        - id: sections_main
                                                            slot: "primary_nav"
                                                                component: "SectionLinks"
                                                                    source: "./sections.skill.md"
                                                                      - id: competencies_v1
                                                                          slot: "competencies"
                                                                              component: "CompetencyGrid"
                                                                                  source: "./competencies.skill.md"
                                                                                    - id: bio_short
                                                                                        slot: "bio"
                                                                                            component: "Bio"
                                                                                                source: "./bio.skill.md"

                                                                                                ## rendering_hints
                                                                                                hero:
                                                                                                  title_as: "h1"
                                                                                                    roles_style: "inline_labels"
                                                                                                      description_as: "body"
                                                                                                      primary_nav:
                                                                                                        layout: "horizontal_pills"
                                                                                                          affordance: "text_with_arrow"
                                                                                                          competencies:
                                                                                                            layout: "radial_cloud"
                                                                                                              count: 16
                                                                                                              bio:
                                                                                                                width: "narrow"
                                                                                                                  align: "left"
                                                                                                                  