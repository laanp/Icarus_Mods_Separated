' Icarus Mod Manager Script File for:
' laanp-HalfCurvedStairs_v1_w230
'-----------------------------------------------------------------------------------------------


'-----------------------------------------------------------------------------------------------
' Defines new buildable items
' Stability - Linked to D_BuildingStability Name: record, which defines building tier strength and stability.
' Type - Linked to Name: records in D_BuildingTypes, for new building type.
' PieceType - blueprint deployment behaviour, all possible entries:
'  - "Floor" (default) 
'  - "Ramp" - Ramps/Stairs/Roofs
'  - "Frame" - Frames, Beams
'  - "Wall" - Walls, Diagonal, Angled, Curved
' Variations - Defines talent requirements and Piece name variations - linked to BuildingPieces Name: record
'-----------------------------------------------------------------------------------------------
\data\Traits\D_Buildable.json
	AddRecord("Rows")
        {
            "Name": "Petes_HalfCurvedStairs_Concrete",
            "Stability": {
                "RowName": "Concrete_General"
            },
            "Type": {
                "RowName": "Concrete"
            },
            "PieceType": "Wall",
            "Variations": [
                {
                    "Requirement": {
                        "RowName": "None",
                        "DataTableName": "D_Talents"
                    },
                    "Piece": {
                        "RowName": "Petes_HalfCurvedStairs_Concrete_InsideUpRight",
                        "DataTableName": "D_BuildingPieces"
                    }
                },
                {
                    "Requirement": {
                        "RowName": "None",
                        "DataTableName": "D_Talents"
                    },
                    "Piece": {
                        "RowName": "Petes_HalfCurvedStairs_Concrete_InsideUpLeft",
                        "DataTableName": "D_BuildingPieces"
                    }
                },
                {
                    "Requirement": {
                        "RowName": "None",
                        "DataTableName": "D_Talents"
                    },
                    "Piece": {
                        "RowName": "Petes_HalfCurvedStairs_Concrete_InsideDnRight",
                        "DataTableName": "D_BuildingPieces"
                    }
                },
                {
                    "Requirement": {
                        "RowName": "None",
                        "DataTableName": "D_Talents"
                    },
                    "Piece": {
                        "RowName": "Petes_HalfCurvedStairs_Concrete_InsideDnLeft",
                        "DataTableName": "D_BuildingPieces"
                    }
                },
                {
                    "Requirement": {
                        "RowName": "None",
                        "DataTableName": "D_Talents"
                    },
                    "Piece": {
                        "RowName": "Petes_HalfCurvedStairs_Concrete_OutsideUpRight",
                        "DataTableName": "D_BuildingPieces"
                    }
                },
                {
                    "Requirement": {
                        "RowName": "None",
                        "DataTableName": "D_Talents"
                    },
                    "Piece": {
                        "RowName": "Petes_HalfCurvedStairs_Concrete_OutsideUpLeft",
                        "DataTableName": "D_BuildingPieces"
                    }
                },
                {
                    "Requirement": {
                        "RowName": "None",
                        "DataTableName": "D_Talents"
                    },
                    "Piece": {
                        "RowName": "Petes_HalfCurvedStairs_Concrete_OutsideDnRight",
                        "DataTableName": "D_BuildingPieces"
                    }
                },
                {
                    "Requirement": {
                        "RowName": "None",
                        "DataTableName": "D_Talents"
                    },
                    "Piece": {
                        "RowName": "Petes_HalfCurvedStairs_Concrete_OutsideDnLeft",
                        "DataTableName": "D_BuildingPieces"
                    }
                }
            ]
        }



'-----------------------------------------------------------------------------------------------
' Defines buildable item in-game names for pieces in building menu (When you hold `R`)
' "AccumulationEnabled" - default (false) - defines whether snow/sand buildup can occur
' Additional entries are custom named pieces, whose RowName: is linked in 2 places:
'   - D_Buildable:   "Variations"..."Piece"..."RowName": 
'   - D_BuildingPieces:  "Name": 
'-----------------------------------------------------------------------------------------------
\data\Building\D_BuildingLookup.json
	AddRecord("Rows")
        {
            "Name": "Petes_HalfCurvedStairs_Concrete_InsideUpRight",
            "PieceName": "NSLOCTEXT(\"D_BuildingLookup\", \"Petes_HalfCurvedStairs_Concrete_InsideUpRight-PieceName\", \"Inside Up Right\")"
        },
        {
            "Name": "Petes_HalfCurvedStairs_Concrete_InsideUpLeft",
            "PieceName": "NSLOCTEXT(\"D_BuildingLookup\", \"Petes_HalfCurvedStairs_Concrete_InsideUpLeft-PieceName\", \"Inside Up Left\")"
        },
        {
            "Name": "Petes_HalfCurvedStairs_Concrete_InsideDnRight",
            "PieceName": "NSLOCTEXT(\"D_BuildingLookup\", \"Petes_HalfCurvedStairs_Concrete_InsideDnRight-PieceName\", \"Inside Down Right\")"
        },
        {
            "Name": "Petes_HalfCurvedStairs_Concrete_InsideDnLeft",
            "PieceName": "NSLOCTEXT(\"D_BuildingLookup\", \"Petes_HalfCurvedStairs_Concrete_InsideDnLeft-PieceName\", \"Inside Down Left\")"
        },
        {
            "Name": "Petes_HalfCurvedStairs_Concrete_OutsideUpRight",
            "PieceName": "NSLOCTEXT(\"D_BuildingLookup\", \"Petes_HalfCurvedStairs_Concrete_OutsideUpRight-PieceName\", \"Outside Up Right\")"
        },
        {
            "Name": "Petes_HalfCurvedStairs_Concrete_OutsideUpLeft",
            "PieceName": "NSLOCTEXT(\"D_BuildingLookup\", \"Petes_HalfCurvedStairs_Concrete_OutsideUpLeft-PieceName\", \"Outside Up Left\")"
        },
        {
            "Name": "Petes_HalfCurvedStairs_Concrete_OutsideDnRight",
            "PieceName": "NSLOCTEXT(\"D_BuildingLookup\", \"Petes_HalfCurvedStairs_Concrete_OutsideDnRight-PieceName\", \"Outside Down Right\")"
        },
        {
            "Name": "Petes_HalfCurvedStairs_Concrete_OutsideDnLeft",
            "PieceName": "NSLOCTEXT(\"D_BuildingLookup\", \"Petes_HalfCurvedStairs_Concrete_OutsideDnLeft-PieceName\", \"Outside Down Left\")"
        }


'-----------------------------------------------------------------------------------------------
' Defines Blueprint, Icon, Audio files for buildable.
' Type' = Linked to BuildingLookup..."Name":
'-----------------------------------------------------------------------------------------------
\data\Building\D_BuildingPieces.json
	AddRecord("Rows")
        {
            "Name": "Petes_HalfCurvedStairs_Concrete_InsideUpRight",
            "Type": {
                "RowName": "Petes_HalfCurvedStairs_Concrete_InsideUpRight"
            },
            "Icon": "/Game/laanp/Petes_HalfCurvedStairs/Icons/ITEM_Petes_HalfCurvedStairs_Concrete_InsideUpRight.ITEM_Petes_HalfCurvedStairs_Concrete_InsideUpRight",
            "Blueprint": "/Game/laanp/Petes_HalfCurvedStairs/BP/BP_Petes_HalfCurvedStairs_Concrete_InsideUpRight.BP_Petes_HalfCurvedStairs_Concrete_InsideUpRight_C",
            "Audio": {
                "RowName": "Concrete"
            }
        },
        {
            "Name": "Petes_HalfCurvedStairs_Concrete_InsideUpLeft",
            "Type": {
                "RowName": "Petes_HalfCurvedStairs_Concrete_InsideUpLeft"
            },
            "Icon": "/Game/laanp/Petes_HalfCurvedStairs/Icons/ITEM_Petes_HalfCurvedStairs_Concrete_InsideUpLeft.ITEM_Petes_HalfCurvedStairs_Concrete_InsideUpLeft",
            "Blueprint": "/Game/laanp/Petes_HalfCurvedStairs/BP/BP_Petes_HalfCurvedStairs_Concrete_InsideUpLeft.BP_Petes_HalfCurvedStairs_Concrete_InsideUpLeft_C",
            "Audio": {
                "RowName": "Concrete"
            }
        },
        {
            "Name": "Petes_HalfCurvedStairs_Concrete_InsideDnRight",
            "Type": {
                "RowName": "Petes_HalfCurvedStairs_Concrete_InsideDnRight"
            },
            "Icon": "/Game/laanp/Petes_HalfCurvedStairs/Icons/ITEM_Petes_HalfCurvedStairs_Concrete_InsideDnRight.ITEM_Petes_HalfCurvedStairs_Concrete_InsideDnRight",
            "Blueprint": "/Game/laanp/Petes_HalfCurvedStairs/BP/BP_Petes_HalfCurvedStairs_Concrete_InsideDnRight.BP_Petes_HalfCurvedStairs_Concrete_InsideDnRight_C",
            "Audio": {
                "RowName": "Concrete"
            }
        },
        {
            "Name": "Petes_HalfCurvedStairs_Concrete_InsideDnLeft",
            "Type": {
                "RowName": "Petes_HalfCurvedStairs_Concrete_InsideDnLeft"
            },
            "Icon": "/Game/laanp/Petes_HalfCurvedStairs/Icons/ITEM_Petes_HalfCurvedStairs_Concrete_InsideDnLeft.ITEM_Petes_HalfCurvedStairs_Concrete_InsideDnLeft",
            "Blueprint": "/Game/laanp/Petes_HalfCurvedStairs/BP/BP_Petes_HalfCurvedStairs_Concrete_InsideDnLeft.BP_Petes_HalfCurvedStairs_Concrete_InsideDnLeft_C",
            "Audio": {
                "RowName": "Concrete"
            }
        },
        {
            "Name": "Petes_HalfCurvedStairs_Concrete_OutsideUpRight",
            "Type": {
                "RowName": "Petes_HalfCurvedStairs_Concrete_OutsideUpRight"
            },
            "Icon": "/Game/laanp/Petes_HalfCurvedStairs/Icons/ITEM_Petes_HalfCurvedStairs_Concrete_OutsideUpRight.ITEM_Petes_HalfCurvedStairs_Concrete_OutsideUpRight",
            "Blueprint": "/Game/laanp/Petes_HalfCurvedStairs/BP/BP_Petes_HalfCurvedStairs_Concrete_OutsideUpRight.BP_Petes_HalfCurvedStairs_Concrete_OutsideUpRight_C",
            "Audio": {
                "RowName": "Concrete"
            }
        },
        {
            "Name": "Petes_HalfCurvedStairs_Concrete_OutsideUpLeft",
            "Type": {
                "RowName": "Petes_HalfCurvedStairs_Concrete_OutsideUpLeft"
            },
            "Icon": "/Game/laanp/Petes_HalfCurvedStairs/Icons/ITEM_Petes_HalfCurvedStairs_Concrete_OutsideUpLeft.ITEM_Petes_HalfCurvedStairs_Concrete_OutsideUpLeft",
            "Blueprint": "/Game/laanp/Petes_HalfCurvedStairs/BP/BP_Petes_HalfCurvedStairs_Concrete_OutsideUpLeft.BP_Petes_HalfCurvedStairs_Concrete_OutsideUpLeft_C",
            "Audio": {
                "RowName": "Concrete"
            }
        },
        {
            "Name": "Petes_HalfCurvedStairs_Concrete_OutsideDnRight",
            "Type": {
                "RowName": "Petes_HalfCurvedStairs_Concrete_OutsideDnRight"
            },
            "Icon": "/Game/laanp/Petes_HalfCurvedStairs/Icons/ITEM_Petes_HalfCurvedStairs_Concrete_OutsideDnRight.ITEM_Petes_HalfCurvedStairs_Concrete_OutsideDnRight",
            "Blueprint": "/Game/laanp/Petes_HalfCurvedStairs/BP/BP_Petes_HalfCurvedStairs_Concrete_OutsideDnRight.BP_Petes_HalfCurvedStairs_Concrete_OutsideDnRight_C",
            "Audio": {
                "RowName": "Concrete"
            }
        },
        {
            "Name": "Petes_HalfCurvedStairs_Concrete_OutsideDnLeft",
            "Type": {
                "RowName": "Petes_HalfCurvedStairs_Concrete_OutsideDnLeft"
            },
            "Icon": "/Game/laanp/Petes_HalfCurvedStairs/Icons/ITEM_Petes_HalfCurvedStairs_Concrete_OutsideDnLeft.ITEM_Petes_HalfCurvedStairs_Concrete_OutsideDnLeft",
            "Blueprint": "/Game/laanp/Petes_HalfCurvedStairs/BP/BP_Petes_HalfCurvedStairs_Concrete_OutsideDnLeft.BP_Petes_HalfCurvedStairs_Concrete_OutsideDnLeft_C",
            "Audio": {
                "RowName": "Concrete"
            }
        }




'---------------------------------------------------------------------------------------------------------------
' Changes to ItemsStatic:
'---------------------------------------------------------------------------------------------------------------
\data\Items\D_ItemsStatic.json
	AddRecord("Rows")
        {
            "Name": "Petes_HalfCurvedStairs_Concrete",
            "Meshable": {
                "RowName": "Mesh_Concrete_Kit"
            },
            "Itemable": {
                "RowName": "Item_Petes_HalfCurvedStairs_Concrete"
            },
            "Interactable": {
                "RowName": "Item"
            },
            "Hitable": {
                "RowName": "Building"
            },
            "Focusable": {
                "RowName": "Focusable_1H"
            },
            "Highlightable": {
                "RowName": "Generic"
            },
            "Actionable": {
                "RowName": "Building"
            },
            "Buildable": {
                "RowName": "Petes_HalfCurvedStairs_Concrete"
            },
            "Usable": {
                "RowName": "Place"
            },
            "Durable": {
                "RowName": "Concrete_Building"
            },
            "Decayable": {
                "RowName": "Decay_General"
            },
            "Audio": {
                "RowName": "ConcreteDeployable"
            },
            "AdditionalStats": {
                "(Value=\"IsInvulnerable_?\")": 1
            },
             "Manual_Tags": {
                "GameplayTags": [
                    {
                        "TagName": "Building.Concrete"
                    },
                    {
                        "TagName": "Audio.Shelter"
                    }
                ]
            },
            "Generated_Tags": {
                "GameplayTags": [
                    {
                        "TagName": "Building.Concrete"
                    },
                    {
                        "TagName": "Audio.Shelter"
                    },
                    {
                        "TagName": "Traits.Meshable"
                    },
                    {
                        "TagName": "Traits.Itemable"
                    },
                    {
                        "TagName": "Traits.Interactable"
                    },
                    {
                        "TagName": "Traits.Hitable"
                    },
                    {
                        "TagName": "Traits.Highlightable"
                    },
                    {
                        "TagName": "Traits.Actionable"
                    },
                    {
                        "TagName": "Traits.Buildable"
                    },
                    {
                        "TagName": "Traits.Usable"
                    },
                    {
                        "TagName": "Traits.Durable"
                    }
                ],
                "ParentTags": []
            }
        }


'---------------------------------------------------------------------------------------------------------------
' Add the item template
'---------------------------------------------------------------------------------------------------------------
\data\Items\D_ItemTemplate.json
	AddRecord("Rows")
        {
            "Name": "Petes_HalfCurvedStairs_Concrete",
            "ItemStaticData": {
                "RowName": "Petes_HalfCurvedStairs_Concrete"
            }
        }


'---------------------------------------------------------------------------------------------------------------
' Modify Itemable:  Descriptions/Icons of In-Game item, as well as Weight/StackSize
'---------------------------------------------------------------------------------------------------------------
\data\Traits\D_Itemable.json
	AddRecord("Rows")
        {
            "Name": "Item_Petes_HalfCurvedStairs_Concrete",
            "DisplayName": "NSLOCTEXT(\"D_Itemable\", \"Item_Petes_HalfCurvedStairs_Concrete-DisplayName\", \"Concrete Curved Half Stairs\")",
            "Icon": "/Game/laanp/Petes_HalfCurvedStairs/Icons/ITEM_Petes_HalfCurvedStairs_Concrete_OutsideUpRight.ITEM_Petes_HalfCurvedStairs_Concrete_OutsideUpRight",
            "Description": "NSLOCTEXT(\"D_Itemable\", \"Item_Petes_HalfCurvedStairs_Concrete-Description\", \"Perfect for curved pieces.\")",
            "FlavorText": "NSLOCTEXT(\"D_Itemable\", \"Item_Petes_HalfCurvedStairs_Concrete-FlavorText\", \"Get Creative!\")",
            "Weight": 0,
            "MaxStack": 100
        }


'--------------------------------------------------------------------------------------------------------- 
' Crafting Changes.... 
'--------------------------------------------------------------------------------------------------------- 
\data\Crafting\D_ProcessorRecipes.json
	AddRecord("Rows")
        {
            "Name": "Petes_HalfCurvedStairs_Concrete",
            "RequiredMillijoules": 1,
            "RecipeSets": [
                {
                    "RowName": "Cement_Mixer",
                    "DataTableName": "D_RecipeSets"
                },
                {
                    "RowName": "Masonry_Bench_T4",
                    "DataTableName": "D_RecipeSets"
                }
            ],
            "Inputs": [
                {
                    "Element": {
                        "RowName": "Steel_Rebar",
                        "DataTableName": "D_ItemsStatic"
                    },
                    "Count": 6,
                    "DynamicProperties": []
                },
                {
                    "Element": {
                        "RowName": "Concrete_Mix",
                        "DataTableName": "D_ItemsStatic"
                    },
                    "Count": 2,
                    "DynamicProperties": []
                }
            ],
            "Outputs": [
                {
                    "Element": {
                        "RowName": "Petes_HalfCurvedStairs_Concrete",
                        "DataTableName": "D_ItemTemplate"
                    },
                    "Count": 1,
                    "DynamicProperties": [],
                    "Alterations": []
                }
            ],
            "Audio": {
                "RowName": "Default"
            }
        }




