"using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;
 
namespace MetotOrtalama
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
        }
 
        public float OrtalamaHesapla(float not1, float not2)
        {
            float sonuc = (not1 + not2) / 2;
            return sonuc;
        }
 
        private void btnHesapla_Click(object sender, EventArgs e)
        {
            float yazili1=Convert.ToSingle(txtYazili1.Text);
            float yazili2 =Convert.ToSingle(txtYazili2.Text);
            
            float ortalama = OrtalamaHesapla(yazili1,yazili2);
            
            lblOrtalama.Text = "Ortalama: "+ortalama.ToString();
        }
    }
}
Convert.ToSingle("elc");
Convert.ToSingle("yazili");
