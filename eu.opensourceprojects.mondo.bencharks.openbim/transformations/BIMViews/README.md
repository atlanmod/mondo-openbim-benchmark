
#BIM views 

We rely on the [MVD](https://www.google.fr/url?sa=t&rct=j&q=&esrc=s&source=web&cd=1&cad=rja&uact=8&ved=0ahUKEwjj1Imo4MnKAhWCVBoKHWF5BMUQFggfMAA&url=http%3A%2F%2Fwww.buildingsmart-tech.org%2Fspecifications%2Fifc-view-definition&usg=AFQjCNHjfu2L9dms9j5vaMxEIZH0Bw8fCA&sig2=2EG_nO2O_SkbiadnbsWo-A&bvm=bv.112766941,d.d2s) specifications to develop views on IFC models. For developing the view we
follow a two-step approach, that users may replicate for future views on BIM on ATL.

1. In a first manual step we produce the view metamodel. MVD specifications enumerate BIM concepts, grouping them by concerns. We select one or more concerns and we create a view
metamodel by (i) copying the full IFC metamodel, (ii) removing the metaclasses that do not appear in the concern.

2. In a second automated step a Higher-Order Transformation from related work ([ATL2Copier](http://www.eclipse.org/atl/atlTransformations/KM32ATLCopier/KM32ATLCopier.zip)) is used to automatically generate, from the view metamodel a view transformation. The resulting view transformation, given a full model conforming to the full IFC metamodel filters out the elements that do not belong to the view.


The *BIMCopier.atl* transformation contains the rules to copy any given bim model into another, while the *IfcWallView.atl* copies only elements belonging to the [IFCWALL-VIEW](http://www.buildingsmart-tech.org/ifc/IFC2x3/TC1/html/ifcsharedbldgelements/lexical/ifcwallstandardcase.htm). 
