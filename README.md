using System;
using System.Drawing;
using System.Windows.Forms;

namespace WinFormsApp1
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
            this.Load += Form1_Load;
        }

        private void Form1_Load(object sender, EventArgs e)
        {
            Button helloButton = new Button();
            helloButton.BackColor = Color.LightBlue;
            helloButton.ForeColor = Color.Black;
            helloButton.Location = new Point(600, 100);
            helloButton.Text = "Привет";
            this.Controls.Add(helloButton);
        }
    }
}
