Typical use cases:

```c#
            string property_name_input1 = TeklaProperties.Assembly.ACTUAL_END_D;
            string property_name_input2 = TeklaProperties.Bolt.BOLT_EDGE_DISTANCE_MIN;
            string property_name_input3 = TeklaProperties.CastUnit.AREA;
            string property_name_input4 = TeklaProperties.Connection.ANG_T;
            string property_name_input5 = TeklaProperties.General.ACTUAL_ENDDATE;

            //// input one of the above inputs to get the property that you are after:
            //// of course you will need to ensure that the Tekla references and directives are added:

            ModelObject mo = selectComponents.Current;
            double a = 0;
            mo.GetReportProperty(property_name_input_1, ref a);

            // of course, put in the relevant input property string.

            Enjoy!

            WARNING: this .cs file has been produced by parsin Tekla's properties file. There may be bugs existing. There are thousands of properties and I didn't have the opportunity to test them all.

            Enjoy!
```