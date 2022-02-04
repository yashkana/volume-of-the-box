# volume-of-the-box
using System;<br>

namespace exersices<br>
{<br>
    class box<br>
    {<br>
        float width;<br>
        float height;<br>
        float length;<br>
        public float Volume<br>
        {<br>
            get { return width * height * length; }<br>
        }<br>
            public box(float width, float height, float length)<br>
        {<br>
            this.width = width;<br>
            this.height = height;<br>
            this.length = length;<br>

        }<br>
        public static float operator +(box box1, box box2)<br>
        {
            return box1.Volume + box2.Volume;<br>
        }
        public override string ToString()<br>
        {<br>

            return "box with width " + width + " height  " + height +" and length  "+ length;<br>

        }<br>
    }<br>
    class OperatorOverlading<br>
    {<br>
        public static void Main()<br>
        {<br>
            box box1 = new box(10, 20, 30);<br>
            box box2 = new box(25, 32, 15);<br>
            Console.WriteLine("Volume of {0} is {1}", box1, box1.Volume);<br>
            Console.WriteLine("Volume of {0} is:{1}", box2, box2.Volume);<br>
            Console.WriteLine("volume after adding boxes:{0}", box1 + box2);<br>
        }<br>
    }<br>
}<br>

OUTPUT

![Screenshot 2022-02-04 053649](https://user-images.githubusercontent.com/98301023/152478264-55283230-fc16-447b-a377-f74d759bf20a.png)







