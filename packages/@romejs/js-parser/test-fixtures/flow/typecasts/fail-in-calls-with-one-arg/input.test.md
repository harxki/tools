# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test packages/@romejs/js-parser/index.test.ts --update-snapshots` to update.

## `flow > typecasts > fail-in-calls-with-one-arg`

```javascript
Program {
  comments: Array []
  corrupt: false
  directives: Array []
  filename: 'input.js'
  hasHoistedVars: false
  interpreter: undefined
  mtime: undefined
  sourceType: 'module'
  syntax: Array [
    'jsx'
    'flow'
  ]
  loc: Object {
    filename: 'input.js'
    end: Object {
      column: 0
      index: 21
      line: 2
    }
    start: Object {
      column: 0
      index: 0
      line: 1
    }
  }
  diagnostics: Array [
    Object {
      origins: Array [Object {category: 'js-parser'}]
      description: Object {
        category: 'parse/js'
        message: PARTIAL_BLESSED_DIAGNOSTIC_MESSAGE {value: 'Function parameter type annotation? Possibly forgot curlies around an object. Possibly forgot async keyword.'}
      }
      location: Object {
        filename: 'input.js'
        mtime: undefined
        sourceType: 'module'
        end: Object {
          column: 18
          index: 18
          line: 1
        }
        start: Object {
          column: 9
          index: 9
          line: 1
        }
      }
    }
  ]
  body: Array [
    ExpressionStatement {
      loc: Object {
        filename: 'input.js'
        end: Object {
          column: 20
          index: 20
          line: 1
        }
        start: Object {
          column: 0
          index: 0
          line: 1
        }
      }
      expression: CallExpression {
        arguments: Array []
        loc: Object {
          filename: 'input.js'
          end: Object {
            column: 19
            index: 19
            line: 1
          }
          start: Object {
            column: 0
            index: 0
            line: 1
          }
        }
        callee: ReferenceIdentifier {
          name: 'funccall'
          loc: Object {
            filename: 'input.js'
            end: Object {
              column: 8
              index: 8
              line: 1
            }
            start: Object {
              column: 0
              index: 0
              line: 1
            }
          }
        }
      }
    }
  ]
}
```