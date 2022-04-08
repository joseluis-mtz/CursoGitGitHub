using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace GUI
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
        }

        private void btnCambio_Click(object sender, EventArgs e)
        {
            string contenido = txtNumero.Text;
            string parte = contenido.Split('.')[1];
            int cantidad = parte.Length;
            string decimales = "";

            if (cantidad == 4)
            {
                //if (parte[0].Equals('0'))
                //{
                //    decimales = "0" + parte[1] + parte[2] + parte[3];
                //}
                //if (parte[0].Equals('0') && parte[1].Equals('0'))
                //{
                //    decimales = "00" + parte[2] + parte[3];
                //}
                //if (parte[0].Equals('0') && parte[1].Equals('0') && parte[2].Equals('0'))
                //{
                //    decimales = "000"+parte[3];
                //}
                //if (parte[0].Equals('0') && parte[1].Equals('0') && parte[2].Equals('0') && parte[3].Equals('0'))
                //{
                //    decimales = "0000";
                //}

            }

            if (cantidad == 3)
            {
                //if (parte[0].Equals('0'))
                //{
                //    decimales = "0" + parte[1] + parte[2] + parte[3];
                //}
                //if (parte[0].Equals('0') && parte[1].Equals('0'))
                //{
                //    decimales = "00" + parte[2] + parte[3];
                //}
                //if (parte[0].Equals('0') && parte[1].Equals('0') && parte[2].Equals('0'))
                //{
                //    decimales = "000" + parte[3];
                //}
                //if (parte[0].Equals('0') && parte[1].Equals('0') && parte[2].Equals('0') && parte[3].Equals('0'))
                //{
                //    decimales = "0000";
                //}
            }
            
            if (cantidad == 2)
            {
                if (parte[0].Equals('0') && parte[1].Equals('0'))
                {
                    decimales = "0000";
                }

                if (parte[0].Equals('0') && parte[1] != '0')
                {
                    decimales = "000" + parte[1];
                }

                if (parte[0] != '0' && parte[1].Equals('0'))
                {
                    decimales = "00" + parte[0] + parte[1];
                }
                if (parte[0] != '0' && parte[1] != '0')
                {
                    decimales = "00" + parte[0] + parte[1];
                }
            }

            if (cantidad == 1)
            {
                if (parte[0].Equals('0'))
                {
                    decimales = "0000";
                }
                else
                {
                    decimales = "000" + parte[0];
                }
            }


            //string cadena = string.Format("{0:0.##00}", contenido);
            lblResultado.Text = decimales;
        }

        private void txtNumero_KeyPress(object sender, KeyPressEventArgs e)
        {
            if ((int)e.KeyChar == (int)Keys.Enter)
            {
                btnCambio.PerformClick();
            }
        }
    }
}
