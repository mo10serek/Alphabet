/*
* Created by: Michael
* Created on: 20-0ct-2015
* Created for: ICS3U
* Daily Assignment – Unit#3-13
* This program show the alphabet
*/

using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace Alphabet
{
    public partial class frmAlphabet : Form
    {
        public frmAlphabet()
        {
            InitializeComponent();
        }

        private void btnStart_Click(object sender, EventArgs e)
        {
            //varibles
            int firstNumber;
            int secondNumber;

            //clear listbox
            this.lstAlphabet.Items.Clear();

            for (firstNumber = 65; firstNumber <= 90; firstNumber++)
            {
                for (secondNumber = 97; secondNumber <= 122; secondNumber++)
                {
                    this.lstAlphabet.Items.Add(Char.ConvertFromUtf32(firstNumber) + " --> " +                                                    Char.ConvertFromUtf32(secondNumber));
                }                   
            }
        }
    }
}
