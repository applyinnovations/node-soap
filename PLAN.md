add attributes to soap definitions

add attributes to
ComplexTypeElement
Element
ExtensionElement
AttributeGroupElement
in node-soap/src/wsdl/elements.ts

this is done by adding attributes to allowed children like

public readonly allowedChildren = buildAllowedChildren([
'annotation',
'complexType',
'simpleType',
]);

public readonly allowedChildren = buildAllowedChildren([
'annotation',
'complexType',
'simpleType',
'attribute',
]);

and adding the AttributeElement class

need to also add attribute group?
