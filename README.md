# Crud
sistema de cadastro

using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace Acai
{
    public partial class telaprincipal : Form
    {
        public telaprincipal()
        {
            InitializeComponent();
        }

        private void telaprincipal_Load(object sender, EventArgs e)
        {

        }

        private void irParaOSeuMenuToolStripMenuItem_Click(object sender, EventArgs e)
        {
            Form1 menu = new Form1();
            menu.ShowDialog();
        }

        private void btn_sair_Click(object sender, EventArgs e)
        {
            Close();
        }

        private void menuPessoalToolStripMenuItem_Click(object sender, EventArgs e)
        {

        }

        private void cadastrarToolStripMenuItem_Click(object sender, EventArgs e)
        {
            teladecadastro menu = new teladecadastro();
            menu.ShowDialog();
        }
    }
}

namespace Acai
{
    public partial class teladecadastro : Form
    {
        public teladecadastro()
        {
            InitializeComponent();
        }

        private void label1_Click(object sender, EventArgs e)
        {

        }

        private void btn_sair2_Click(object sender, EventArgs e)
        {
            Close();
        }

        private void teladecadastro_Load(object sender, EventArgs e)
        {

        }
    }
}

namespace Acai

{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
            txt_tipo.Enabled = false;
            txt_frutas.Enabled = false;
            txt_tamanho.Enabled = false;
            txt_preco.Enabled = false;
            txt_precototal.Enabled = false;
        }

        private void maskedTextBox1_MaskInputRejected(object sender, MaskInputRejectedEventArgs e)
        {

        }

        private void btn_add_Click(object sender, EventArgs e)
        {
            MessageBox.Show("Crie seu menu pessoal preenchendo as informações acima ");
            txt_tipo.Enabled = true;
            txt_frutas.Enabled = true;
            txt_tamanho.Enabled = true;
            txt_preco.Enabled = true;
            txt_precototal.Enabled = true;
        }

        private void btn_salvar_Click(object sender, EventArgs e)
        {
            MessageBox.Show("Menu pessoal salvo com sucesso");

        }

        private void Form1_Load(object sender, EventArgs e)
        {

        }

        private void btn_sair3_Click(object sender, EventArgs e)
        {
            Close();
        }
    }
}
namespace Acai
{
    static class Program
    {
        /// <summary>
        /// The main entry point for the application.
        /// </summary>
        [STAThread]
        static void Main()
        {
            Application.EnableVisualStyles();
            Application.SetCompatibleTextRenderingDefault(false);
            Application.Run(new telaprincipal());
        }
    }
}
