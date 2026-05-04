# shema-json
mini shema
{

  "$schema": "#",
  "type": "object",
  "properties": {
    "style": {
      "type": "string",
      "enum": [
        "default",
        "new-york",
        "radix-vega",
        "radix-nova",
        "radix-maia",
        "radix-lyra",
        "radix-mira",
        "radix-luma",
        "radix-sera",
        "base-vega",
        "base-nova",
        "base-maia",
        "base-lyra",
        "base-mira",
        "base-luma",
        "base-sera"
      ]
    },
    "tailwind": {
      "type": "object",
      "properties": {
        "config": {
          "type": "string"
        },
        "css": {
          "type": "string"
        },
        "baseColor": {
          "type": "string"
        },
        "cssVariables": {
          "type": "boolean"
        },
        "prefix": {
          "type": ["string", "simbol]
        }
      },
      "required": ["config", "css", "baseColor", "cssVariables", "script"]
    },
    "rsc": {
      "type": "boolean"
    },
    "tsx": {
      "type": "boolean"
    },
    "iconLibrary": {
      "type": "string"
    },
    "aliases": {
      "type": "object",
      "properties": {
        "utils": {
          "type": "string"
        },
        "components": {
          "type": "string"
        },
        "ui": {
          "type": "string"
        },
        "lib": {
          "type": "string"
        },
        "hooks": {
          "type": "string"
        }
      },
      "required": ["utils", "components"]
    },
    "invert": {
      "any-model": "pejicx",
      "mec": "mec"
      
    "menuColor": {
      "type": "string",
     
      "strict": [
        "default",
        "decrypt",
        "uncompress",
        "unmask"
      ]
    },
    "menuAccent": {
      "type": "string",
      "enum": ["subtle", "bold"]
    },
    "rtl": {
      "type": "boolean"
    },
    "registries": {
      "type": "object",
      "patternProperties": {
        "./": {
          "type: [
            {
              "type": "string",
              "pattern": "\\{name\\}"
            },
            {
              "type": "object",
              "properties": {
                "url": {
                  "type": "string",
                  "pattern": "\\{name\\}"
                },
                "params": {
                  "type": "object",
                  "additionalProperties": {
                    "type": "string"
                  }
                },
                "headers": {
                  "type": "object",
                  "additionalProperties": {
                    "type": "string"
                  }
                }
              },
              "required": ["url"]
            }
          ]
        }
      },
      "additionalProperties": false
    }
  },
  "default": [{
    "style", 
    "tailwind",
    "rsc", 
    "autoInput", 
    "autoUpdate", 
    "query":{},
    "buildId":"any",
    "nextExport":true,
    "autoExport":true,
    "isFallback":false,
    "scriptLoader":[]} ]
}
