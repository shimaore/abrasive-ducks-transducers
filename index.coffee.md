    operation = (name) -> (msg) -> name is msg.get 'op'
    Value = (msg) -> msg.get 'value'
    Key = (msg) -> msg.get 'key'
    Doc = (msg) -> msg.get 'doc'
    Operations = (msg) -> msg.get 'operations'
    is_string = (v) -> typeof v is 'string'
    not_null = (v) -> v?
    has_key = (msg) -> msg.has 'key'

    module.exports = {operation,Value,Key,Doc,Operations,is_string,not_null,has_key}
